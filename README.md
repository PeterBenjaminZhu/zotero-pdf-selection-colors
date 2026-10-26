# PDF Selection Colors · PDF 选中底色

为 Zotero PDF 阅读器自定义临时文字选择底色，提供 Everforest 强调绿、莫兰迪预设、自定义颜色和不透明度调节。

Customize temporary PDF text-selection colors in Zotero, with Everforest and Morandi presets, a custom color picker, and adjustable opacity.

## 兼容性

- 当前版本：**1.0.2**。
- 适用版本：**Zotero 10.0.6**，已在 Windows 上检查。
- 安装包仅声明支持 Zotero 10.0.6。其他 Zotero 版本需要重新检查适配；macOS 与 Linux 尚未验证。

## 下载与安装

1. [下载 pdf-selection-colors-1.0.2.xpi](https://github.com/PeterBenjaminZhu/zotero-pdf-selection-colors/raw/refs/heads/main/pdf-selection-colors-1.0.2.xpi)。请保存 `.xpi` 文件。
2. 在 Zotero 中打开 **工具 → 插件**。
3. 点击齿轮按钮，选择 **Install Plugin From File… / 从文件安装插件**，选择下载的 `.xpi`。
4. 安装后重新启动一次 Zotero。

无需修改 Zotero 安装文件或现有主题文件。插件采用手动下载安装包的更新方式，目前没有自动更新服务。

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

已检查单词、多行、跨段落及跨页选择、包含公式的正文、深色与临时白底页面、复制和取消选择、引用链接跳转、高亮和下划线原色、分屏、独立阅读窗口、另一篇论文、重启后的设置保留，以及停用恢复。

短距离翻页与选择处理对比未发现明显新增卡顿。检查基于本机现有公开论文，结果不能代表全部论文、缩放比例、设备或长时间使用情况；扫描 PDF 尚未检查。未覆盖其他插件的全部功能。

## 文件与源码

仓库提供安装包、使用说明、版本记录和校验文件。`.xpi` 使用 ZIP 格式，包含插件的 JavaScript、界面、样式与配置文件，解压即可查看源码。

安装包 SHA-256：

```text
3139937e6644b85477b29a1da34d75d6cb7ecf97d1362e4cbfefe2d3bb0cfdc3
```

## 反馈

遇到问题时，请在 [Issues](https://github.com/PeterBenjaminZhu/zotero-pdf-selection-colors/issues) 中提供 Zotero 版本、操作系统、复现步骤，以及是否使用深色阅读主题。

## License

[MIT License](LICENSE)
