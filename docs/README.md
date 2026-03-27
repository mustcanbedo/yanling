# 文档说明

本目录存放**可公开访问**的合规与说明类文档，供 Chrome 网上应用店、官网等填写 URL 时使用。

| 文件 | 用途 |
|------|------|
| [privacy-policy.md](privacy-policy.md) | 隐私政策正文；商店「隐私政策」字段请填该文件在 GitHub 上的 **blob** 浏览链接（HTTPS）。 |

**与扩展内文案同步**：隐私政策正文应与 comment_copilot 仓库 `apps/extension/sidepanel/legal-content.tsx` 中 `PRIVACY_POLICY` 保持一致；联系邮箱以同仓库 `constants.ts` 的 `FEEDBACK_EMAIL` 为准。更新扩展内文案后，请同步修订本文件并更新 `privacy-policy.md` 顶部的「更新日期」。

《服务条款》当前以扩展包内「驭灵」展示为准。若需要在本仓库公开发布条款，可新增 `terms-of-service.md`，并在根目录 README「法律与合规」中补充 blob 链接说明。
