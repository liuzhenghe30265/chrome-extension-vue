# chrome-extension-vue

开发 Chrome 浏览器插件。

[Vue 版本](https://18055975947.github.io/extension/teach/vue-chrome.html
)

## 生成 dist 文件夹

```bash
npm run build
```

## 热加载

```bash
npm run watch-build
```

## 启动本地服务

VScode 插件 Live Server 启动一个服务，右下角 Go Live；

服务地址配置到 manifest.json、src\background\service-worker.ts 文件中。

## 加载扩展程序

chrome://extensions/ 进入管理扩展程序，加载已解压的扩展程序，找到 dist 目录并加载。

固定扩展程序显示弹窗。

访问本地服务显示 content 内容。