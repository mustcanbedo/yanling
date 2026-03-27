# 言灵 Yanling

Chrome 扩展（小红书 / 哔哩哔哩 / 抖音等站点评论区 AI 助手）。**本仓库不存放源码**，仅用于三件事：

| 用途 | 链接 |
|------|------|
| **隐私政策**（商店等场景填公开 URL） | 文档：[docs/privacy-policy.md](docs/privacy-policy.md) · 商店请填 **blob** 页，例如 `https://github.com/mustcanbedo/yanling/blob/main/docs/privacy-policy.md` |
| **反馈** | [Issues](https://github.com/mustcanbedo/yanling/issues) |
| **安装包** | [Releases](https://github.com/mustcanbedo/yanling/releases) · [**下载 v0.1.0（zip）**](https://github.com/mustcanbedo/yanling/archive/refs/tags/v0.1.0.zip) |

GitHub 按**标签**打包的是整个仓库快照；扩展 zip 若在解压后的 `packages/chrome-mv3-prod.zip`（或解压该 zip 得到扩展目录），再按下方侧载。**侧载**：在 Chrome 打开 `chrome://extensions/` → 开发者模式 →「加载已解压的扩展程序」→ 选中**含 `manifest.json` 的扩展目录**（若当前只有 `.zip`，需先解压出目录）。

发新版时请新建标签（如 `v0.1.1`）并把上面表格里的链接中的版本号改成新标签。

扩展构建与源码在 [**comment_copilot**](https://github.com/mustcanbedo/comment_copilot) 的 `apps/extension/`。
