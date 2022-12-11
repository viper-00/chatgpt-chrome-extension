# ChatGPT Chrome 扩展 🤖 ✨

此 Chrome 扩展支持将内容写入 [ChatGPT](https://chat.openai.com) 并输出。例如将推文写入、修改邮件、解决代码 BUG 或者是任何你想问的问题。在这种情况下不需要离开网站即可获得问题的答案。此扩展支持集成插件和一些与 ChatGPT API 交互的功能。

![](https://i.imgur.com/CPMOyG7.gif)

## 安装

首先拷贝项目到本地文件夹

然后安装依赖

```bash
npm install
```

拷贝 `.env-example` 并配置到 `.env` 文件，填入 ChatGPT session token，具体获得方式<a href="https://github.com/transitive-bullshit/chatgpt-api#session-tokens" target="_blank">在这</a>。

运行服务并与 Chrome 扩展进行通信和交换

```bash
node server.js
```

添加 Chrome 扩展流程

1. 去到 Google Chrome 浏览器的 chrome://extensions 的位置
2. 点击并打开开发者模式
3. 点击 "Load Unpacked"
4. 选择项目主目录的 `/extension` 文件夹

现在在 Chrome 的主页面就能看到 "Ask ChatGPT" 了。

## 插件

插件能够与 ChatGPT 回复的规则和解析进行自定义转换，处理的结果会返回给客户端

[Default](/plugins/Default.js) - 设置默认的交互规则 🧑‍🏫

[Image](/plugins/Image.js) - 当查图片时，告诉 ChatGPT 替换成 [Lexica](http://lexica.art) 📸 已有的图片库中的图片，并返回相应图片。

任何你觉得有用的插件，都可以提交 PR 并集成到现有项目中。🤝

## 相关

非常感谢 <a href="https://twitter.com/transitive_bs">Travis Fischer</a> 开发了 [chatgpt-api](https://github.com/transitive-bullshit/chatgpt-api)

## 开源证书

MIT © Gabe Ragland (follow me on <a href="https://twitter.com/gabe_ragland">Twitter</a>)
