### 效果

左上角有版本切换的按钮，点击即可切换文档版本

### 关键配置
`mutiversion` 配置多版本切换，使用此功能需要切换到新的分支(此分支专门用于生成文档)，在新分支的配置文件中添加此配置项

`mutiversion.docbranch` 配置新分支(专门用于生成文档的分支)名称

`mutiversion.versions` 版本信息

`mutiversion.versions[*].name` 版本名称

`mutiversion.versions[*].branch` 版本所在的git分支

```
"mutiversion": { // 配置多版本切换，使用此功能需要切换到新的分支(此分支专门用于生成文档)，在新分支的配置文件中添加此配置项
    "docbranch": "doc", // 新分支(专门用于生成文档的分支)名称
    "versions":[{
        "name": "1.0", // 需要生成的版本名称
        "branch": "v0.0.1" // 需要生成的版本所在的git分支
    },{
        "name": "2.0",
        "branch": "v0.0.2"
    },{
        "name": "3.0",
        "branch": "v0.0.3"
    }] // 需要切换的版本信息
},
```
