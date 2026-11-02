# PDF Selection Colors · PDF 选中底色

为 Zotero PDF 阅读器自定义临时文字选择底色，提供 Everforest 强调绿、莫兰迪预设、自定义颜色和不透明度调节。

Customize temporary PDF text-selection colors in Zotero, with Everforest and Morandi presets, a custom color picker, and adjustable opacity.

## 兼容性

- 当前版本：**1.0.4**。
- 适用版本：**Zotero 10.0.6–10.0.7**。10.0.6 已在 Windows 上检查；1.0.3 在 10.0.7 上由使用者确认实际运行正常。
- 安装包仅声明支持 Zotero 10.0.6–10.0.7。其他 Zotero 版本需要重新检查适配；macOS 与 Linux 尚未验证。

## 下载与安装

1. [下载 pdf-selection-colors-1.0.4.xpi](https://github.com/PeterBenjaminZhu/zotero-pdf-selection-colors/raw/refs/heads/main/pdf-selection-colors-1.0.4.xpi)，保存 `.xpi` 文件。
2. 在 Zotero 中打开 **工具 → 插件**。
3. 点击齿轮按钮，选择 **Install Plugin From File… / 从文件安装插件**，选择下载的 `.xpi`。
4. 安装后重新启动一次 Zotero。

升级保留已经保存的颜色和不透明度，无需修改现有主题文件。

## 自动更新

从 **1.0.4** 开始，插件使用 Zotero 自带的更新功能。版本信息和安装包由本 GitHub 仓库提供，更新时核对安装包的 SHA-256 校验值。

首次安装 1.0.4 会开启此插件的自动更新。以后可以在 **工具 → 插件 → PDF 选中底色 → 详情** 中调整自动更新设置；插件会保留之后的手动选择。

也可以通过插件管理中的 **Check for Updates / 检查更新** 主动检查。自动更新的检查和安装时间由 Zotero 安排；网络需要能够访问 GitHub 的文件下载服务。

**1.0.3 及更早版本需要先手动安装一次 1.0.4**，之后即可通过 Zotero 获取本仓库发布的兼容版本。

版本信息：[updates.json](https://raw.githubusercontent.com/PeterBenjaminZhu/zotero-pdf-selection-colors/main/updates.json)。

## 使用

打开 **工具 → PDF 选中底色…**。

默认采用 **强调绿 `#A7C080`，不透明度 25%**。调整后自动保存，立即应用到已打开的 PDF；重新启动后保留设置。平时调整颜色无需重启 Zotero。

| 预设 | 颜色代码 |
| --- | --- |
| Everforest 强调绿 | `#A7C080` |
| 莫兰迪灰绿 | `#A3B5A4` |
| 莫兰迪灰蓝 | `#9CAFB7` |
| 莫兰迪灰紫 | `#B3A3B5` |
| 莫兰迪灰粉 | `#C2A3A3` |
| 莫兰迪灰褐 | `#B8AD96` |

支持自定义选色和六位颜色代码输入。不透明度提供滑动条与数字输入，范围为 **0%–100%**，数值越大，底色越明显。0% 完全透明，100% 完全不透明。

点击 **恢复默认**，恢复强调绿和 25% 不透明度。

## 修改范围

插件只调整普通文字选择时的临时底色。正文、公式、图表、已有批注、高亮工具和下划线工具继续使用原有颜色。

论文及 Zotero 原有的链接底色、鼠标经过提示保持原样。链接改为灰绿后，会与同色的文字选择预设重复，选择链接时也容易发生底色重叠，因此当前版本保留原链接效果。

## 停用与卸载

在 **工具 → 插件** 中停用 **PDF 选中底色**，即可恢复 Zotero 原有的蓝色选择效果；重新启用后恢复保存的配色。也可通过插件管理移除此插件。现有主题继续保留。

## 检查范围与限制

1.0.2 在 Zotero 10.0.6 中已检查单词、多行、跨段落及跨页选择、包含公式的正文、深色与临时白底页面、复制和取消选择、引用链接跳转、高亮和下划线原色、分屏、独立阅读窗口、另一篇论文、重启后的设置保留，以及停用恢复。

上述检查中的短距离翻页与选择处理对比未发现明显新增卡顿。检查基于本机现有公开论文，结果不能代表全部论文、缩放比例、设备或长时间使用情况；扫描 PDF 尚未检查。未覆盖其他插件的全部功能。

1.0.3 更新了支持版本声明与启动时的版本检查，由使用者在 Zotero 10.0.7 中确认实际运行正常；本次未重新执行上述全部检查。1.0.4 增加自动更新配置，配色及阅读功能文件与 1.0.3 一致。

## 文件与源码

仓库提供安装包、使用说明、版本记录、校验文件和自动更新版本信息。`.xpi` 使用 ZIP 格式，包含插件的 JavaScript、界面、样式与配置文件，解压即可查看源码。

当前安装包 SHA-256：

```text
6db29959b18e4ee075c8a354243b841b625aac82bde23660829f17abd3c18aac
```

## 发布新版本

维护者发布新版时，应同时上传对应版本的安装包，并更新 `updates.json` 中的版本、下载地址、校验值和适用 Zotero 版本范围；同时更新 README、版本记录和 `SHA256SUMS`。仅上传安装包时，Zotero 不会发现新版本。已经发布的版本安装包应保留原文件内容。

## 反馈

遇到问题时，请在 [Issues](https://github.com/PeterBenjaminZhu/zotero-pdf-selection-colors/issues) 中提供 Zotero 版本、操作系统、复现步骤，以及是否使用深色阅读主题。

## License

[MIT License](LICENSE)
