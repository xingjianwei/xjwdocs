# vscode

### 安装markdown插件

vscode默认是支持markdown的，只需要装一个预览插件神器：Markdown Preview Enhanced。 
除了常规的功能外，特别要提出的是两个功能： 

### 将Preview 设置为github风格

vscode 默认的将Preview预览风格是黑黑的，如上面的截图。如果想更改为github风格的样式，请执行如下步骤：

a.下载github风格的[css](manifests/markdown-github.css)到本地，并放置相应的目录，本文推荐放置在vscode安装目录里，如D:/Program Files (x86)/Microsoft VS Code/resources/app/extensions/markdown/media/。
b.设置用户配置文件,File --> Preferences --> Settings,添加如下配置信息，请填入你下载的css文件的路径和名称（我这里的文件名叫userStyle.css）。
  "markdown.styles": [
      "file:///D:/Program Files (x86)/Microsoft VS Code/resources/app/extensions/markdown/media/userStyle.css"
  ],