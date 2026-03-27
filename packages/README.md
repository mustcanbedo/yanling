# 安装包目录（`packages/`）

扩展**只在源码仓库 comment_copilot 内构建**，路径：`apps/extension/`。

| 产物 | 命令 | 路径 |
|------|------|------|
| 生产目录（未压缩） | `npm run build` | `build/chrome-mv3-prod/` |
| 侧载 zip | `npm run package` | `build/chrome-mv3-prod.zip` |
| 商店上架 zip（无 localhost 等） | `npm run package:store` | `build/chrome-mv3-prod.zip`（覆盖） |

完整说明见 comment_copilot 的 [`docs/extension-packaging.md`](https://github.com/mustcanbedo/comment_copilot/blob/main/docs/extension-packaging.md)；商店上架流程见同仓库 [`docs/chrome-web-store.md`](https://github.com/mustcanbedo/comment_copilot/blob/main/docs/chrome-web-store.md)。

---

## 本目录用途

`packages/` 用于**可选暂存**：把构建好的 zip 拷到这里，便于交接或临时备份。**不要**在 yanling 仓库里执行 `npm run build` / `package`。

- **GitHub Releases（推荐对外 zip）**：上传附件时建议使用固定文件名 **`chrome-mv3-prod.zip`**，与根目录 README 中 `releases/latest/download/chrome-mv3-prod.zip` 直链一致。
- **提交到 git**：`.zip` / `.crx` 可以纳入版本控制；大文件会快速增大仓库体积，重要版本请优先以 **Release 附件**为主备份。
- **Chrome 网上应用店**：分发以商店安装为准；商店包请用 comment_copilot 的 `npm run package:store` 生成后再上传开发者后台。

---

## 侧载安装（给最终用户简述）

1. 解压 `chrome-mv3-prod.zip`。  
2. Chrome 打开 `chrome://extensions/`，打开「开发者模式」。  
3. 「加载已解压的扩展程序」→ 选中解压后**包含 `manifest.json` 的那一层目录**。

常见问题（如清单错误、路径含中文等）见 comment_copilot `docs/extension-packaging.md` 文末「常见问题」。
