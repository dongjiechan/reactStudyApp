# reactdemo

## Folder Structure

After creation, your project should look like this:

```
my-app/
  README.md
  node_modules/
  package.json
  public/
    index.html
    favicon.ico
  src/
    App.css
    App.js
    App.test.js
    index.css
    index.js
    logo.svg
```

您可以删除或重命名其他文件。

你可以创建在` SRC `子目录。更快的重建，只有文件里面` SRC `进行WebPACK。<br>

你需要**把JS和CSS文件里面` SRC ` **，否则WebPACK不会看到他们。

只有“公共”中的文件可以从“公共”或“索引”中使用。

请阅读下面的说明，以便使用JavaScript和HTML的资产。

不过，您可以创建更高级的目录。

它们不会包含在产品构建中，因此您可以将它们用于文档之类的东西。

## Available Scripts

In the project directory, you can run:

### `npm start`

启动项目<br>
Open [http://localhost:3000](http://localhost:3000) to view it in the browser.

### `npm test`

在交互监视模式下启动测试运行器。<br>
看到[ ]的部分（#运行测试，运行测试）的更多信息。

### `npm run build`

打包.<br>
它正确地在生产模式中捆绑反应并优化构建以获得最佳性能。

构建压缩文件

看到[部署]的部分（#部署）的更多信息。

### `npm run eject`

### Visual Studio Code
你需要最新版本的[ VS代码]

然后把'launch.json' 文件放在`.vscode `应用程序的根目录文件夹。

```json
{
  "version": "0.2.0",
  "configurations": [{
    "name": "Chrome",
    "type": "chrome",
    "request": "launch",
    "url": "http://localhost:3000",
    "webRoot": "${workspaceRoot}/src",
    "sourceMapPathOverrides": {
      "webpack:///src/*": "${webRoot}/*"
    }
  }]
}
```


