## 扩展示例配置说明

### 效果
在控制台中查看Console有两个js文件的输出。

在控制台中查看Elements有两个css文件的样式。

在控制台中查看Network可以看到自定义的扩展文件。

### 关键配置

`resources` 中配置路径，可以拷贝文件夹到生成文档的目录中.

其中`scripts`与`plugins`字段配置的文件将分别以js/css文件的形式被引入到每个页面的尾部。

```
"options": {
    "insertCSS": ["./style/insert0.css","./style/insert1.css"],  // 配置css路径，可覆盖默认样式； 相对路径需要配置resources路径
    "insertJS": ["./scripts/insert.js", "./plugins/plugin.js"]  // 配置js路径；相对路径需要配置resources路径
},
"resources": { //将配置的文件夹拷贝至生成文档的文件夹下
    "img": "./images", // key值为source
    "style": "./style/", // 指定insertCSS后，配置css的目录
    "scripts": "./scripts/", // 指定insertJS后，配置js的目录
    "plugins": "./plugins/" // 指定insertJS后，配置js的目录
}
```
