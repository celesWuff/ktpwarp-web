# ktpwarp-web

ktpWarp：课堂派自动签到 - Web 客户端

在任何能联网的设备上，查看您 ktpWarp 服务器的签到情况，在网页中扫码，然后提交二维码签到。

了解 ktpwarp-server: https://github.com/celesWuff/ktpwarp-server

## 注意

ktpWarp 仍处于 Beta 阶段，这代表 ktpWarp 尚未在生产环境中得到大规模的验证。

因此，ktpWarp 仍可能存在着未知的 Bug 或签到“脱靶”。如果您发现了 Bug，欢迎您在 Issues 中报告。

## 开始使用

https://celeswuff.github.io/ktpwarp-web/

## 限制

- 扫码器的识别率很低。如需扫码，强烈建议使用其他方案。

  - iOS：[ktpwarp-ios-mitm](https://github.com/celesWuff/ktpwarp-ios-mitm)

  - Android：[ktpwarp-android](https://github.com/celesWuff/ktpwarp-android)

以下限制来自于现代浏览器的安全策略。

- 部署在 `https://`（加密）网站上的 ktpwarp-web，不能访问 `ws://`（未加密）的 ktpwarp-server。**反之亦然。**

- 在本地运行的 ktpwarp-web，无法使用扫码功能。即使可以打开摄像头，也无法识别出二维码。

## 隐藏功能

- 在 URL 中添加 `?server` 参数，可以自动连接到指定的 ktpwarp-server。这个功能对于 [iOS MITM 模块](https://github.com/celesWuff/ktpwarp-ios-mitm) 非常有用。

  - 例如：`https://celeswuff.github.io/ktpwarp-web/?server=wss://example.com/our-ktpwarp-server`

## 许可证

MIT License
