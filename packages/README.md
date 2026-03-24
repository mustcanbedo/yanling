# 安装包目录

扩展**实际构建**在源码仓库 **comment_copilot** 内完成：

- 路径：`apps/extension/build/`
- 生产目录：`build/chrome-mv3-prod`（`npm run build`）
- 单文件包：`build/chrome-mv3-prod.zip`（`npm run package`）

详见 comment_copilot 仓库的 [`docs/extension-packaging.md`](https://github.com/mustcanbedo/comment_copilot/blob/main/docs/extension-packaging.md)（若仓库为私有，请在本机打开对应文档）。

---

本仓库的 **`packages/`** 只做**可选暂存**：把上述 zip（或自行打的包）拷到这里，方便上传 [GitHub Releases](https://github.com/mustcanbedo/yanling/releases) 或交接；**不要**在 yanling 仓库里执行构建。

- **对外分发**：仍以 [GitHub Releases](https://github.com/mustcanbedo/yanling/releases) 或 Chrome 网上应用店为准。
- **提交到本仓库**：`packages/` 下的 `.zip` / `.crx` **可以**纳入版本控制；若每个版本都提交大包，仓库体积会涨得快，重要版本可额外上传到 Release 附件作备份。
