# CrossAnki 个人固件与 OTA

CrossAnki 是基于 **[CrossMux（0x1abin/crossmux）](https://github.com/0x1abin/crossmux)** 修改的个人使用固件，面向 **Waveshare ESP32-S3-ePaper-3.97（微雪 3.97 英寸墨水屏）**。

感谢 CrossMux 上游项目及贡献者提供阅读器、硬件适配和应用基础。CrossAnki 是个人定制版本，不是 CrossMux 官方发布。

## 软件来源与版本

| 项目 | 说明 |
| --- | --- |
| 软件上游 | [0x1abin/crossmux](https://github.com/0x1abin/crossmux) |
| 当前个人版本 | `crossanki-1.3b` |
| 当前上游基线 | CrossMux Nightly 1512e8e #171 |
| 上游提交 | `1512e8e049f2b1a4efc7c004a5b1a93cbc5e3f9f` |
| 上游发布 | [CrossMux Nightly 1512e8e #171](https://github.com/0x1abin/crossmux/releases/tag/nightly-build-1512e8e049f2b1a4efc7c004a5b1a93cbc5e3f9f-171-1) |
| 硬件 target / board tag | `waveshare_epaper_397` |

后续版本的具体上游提交、构建提交、适用硬件与校验值，以各 Release 附带的 `release-metadata.json` 和 `SHA256SUMS` 为准。

## 个人定制内容

在 CrossMux 基础上保留阅读和查词功能，加入离线 Anki 记忆卡、卡片图片与音频、本地 MP3 Music App、阅读时后台播放以及个人 OTA 更新，并按个人需求裁剪娱乐应用。具体功能和修正以各版本说明为准。

本固件用于作者自己的微雪设备。当前发布仅面向上述微雪 3.97 硬件，不能作为其他同为 ESP32-S3 的板子的通用固件。

## 仓库用途与更新

本仓库用于公开分发编译好的个人固件、版本元数据、校验文件和 OTA 清单。个人项目源码在私人仓库维护；上游源码请访问 [CrossMux](https://github.com/0x1abin/crossmux)。

- [个人固件 Releases](https://github.com/lalaniu85/crossanki-ota/releases)
- [CrossAnki 1.3b](https://github.com/lalaniu85/crossanki-ota/releases/tag/crossanki-build-crossanki-1.3b-1512e8e-b544e83)
- [个人 OTA 最新清单](https://github.com/lalaniu85/crossanki-ota/releases/download/crossanki-nightly/latest.json)

`crossanki-nightly` 保存滚动更新清单；具体固件位于独立版本 Release。已配置此个人 OTA 渠道的设备可通过固件更新菜单检查新版本。
