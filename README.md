# 言灵 Yanling

> 小红书 / 哔哩哔哩 / 抖音 等评论区 AI 助手 —— 用 AI 回评论，点燃言灵力

## 本仓库做什么

- **Release**：在 [Releases](https://github.com/mustcanbedo/yanling/releases) 发布可下载的扩展包（侧载 zip）。
- **反馈**：通过 [Issues](https://github.com/mustcanbedo/yanling/issues) 收集 Bug、建议与使用反馈。
- **合规**：在 [`docs/`](docs/) 提供面向 Chrome 网上应用店等场景的**公开文档**（如隐私政策）。

扩展**源代码与构建**在独立仓库 **comment_copilot**（路径 `apps/extension/`）。本仓库**不包含**言灵扩展的源码。

**文档索引**：根目录本文件 · [`packages/README.md`](packages/README.md)（安装包与发版约定）· [`docs/README.md`](docs/README.md)

---

## 安装与下载

### Chrome 网上应用店

扩展上架后，将下方链接替换为商店里的**扩展详情页**（形如 `https://chromewebstore.google.com/detail/...`）。

- 当前占位：[Chrome 网上应用店](https://chromewebstore.google.com/)

### 侧载 zip（开发者模式）

1. 扩展包由 **comment_copilot** 在 `apps/extension/` 执行 `npm run package` 生成 **`build/chrome-mv3-prod.zip`**（与附件名一致即可上传）。
2. 在 [Releases](https://github.com/mustcanbedo/yanling/releases) 新建版本时，上传附件且**文件名为 `chrome-mv3-prod.zip`**，与 README 直链一致。
3. 用户下载后解压，在 Chrome 打开 `chrome://extensions/` → 开启「开发者模式」→「加载已解压的扩展程序」→ 选择**含 `manifest.json` 的文件夹**。

**一键下载（最新 Release 附件）**：

- [**下载 chrome-mv3-prod.zip**](https://github.com/mustcanbedo/yanling/releases/latest/download/chrome-mv3-prod.zip)

> 若尚未上传同名附件，上述链接会 404；上架商店后仍可并行保留 Release 侧载渠道。

### 备用：仓库内的 zip

若已将 `chrome-mv3-prod.zip` 提交到 [`packages/`](packages/) 并推送到默认分支，可使用 raw 直链（默认分支为 `main` 时）：

- <https://github.com/mustcanbedo/yanling/raw/main/packages/chrome-mv3-prod.zip>

分支不是 `main` 时请把 URL 中的分支名改成你的默认分支；文件未提交时会 404。

---

## 反馈与支持

- **GitHub**：[提交 Issue](https://github.com/mustcanbedo/yanling/issues)（支持模板：Bug、功能建议、意见反馈）。
- **产品内**：扩展侧栏「驭灵」→「关于」→「意见反馈」。

构建与打包细节见 **comment_copilot** 的 [`docs/extension-packaging.md`](https://github.com/mustcanbedo/comment_copilot/blob/main/docs/extension-packaging.md)（仓库私有时在本机打开对应路径）。

---

## 版本说明

扩展版本号以 **comment_copilot** `apps/extension/package.json` 的 `version` 与扩展内「关于」为准；本仓库 **Release 标签**建议与之对齐（例如 `v0.1.0`），便于用户对照。

---

## 法律与合规（公开链接）

Chrome 网上应用店等需要填写的**隐私政策 URL**须为 **HTTPS、无需登录即可访问**：

- 文档：[隐私政策](docs/privacy-policy.md)
- 商店中请填 **GitHub 浏览链接（blob）**，例如：  
  `https://github.com/mustcanbedo/yanling/blob/main/docs/privacy-policy.md`  
  （默认分支不是 `main` 时，将链接中的分支名改为实际默认分支。）

《服务条款》全文见安装包内「驭灵」法律文档。若需在仓库同步公开条款，可新增 `docs/terms-of-service.md` 并同样使用 `blob/...` 链接。
