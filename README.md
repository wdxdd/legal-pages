# legal-pages

Public legal & support pages for my apps (privacy policy, support), served via GitHub Pages.

公开的 App 法律与支持页面（隐私政策、支持页），通过 GitHub Pages 托管。

## Structure / 目录结构

```
legal-pages/
├── index.html          # 项目索引 / project index
└── <project>/          # 每个项目一个目录
    ├── index.html      # 项目概览 / overview
    ├── privacy.html    # 隐私政策 / privacy policy
    └── support.html    # 支持页 / support
```

## Projects / 项目

| Directory | App | Pages |
|---|---|---|
| `musepearl/` | MusePearl · 灵珠 | [privacy](./musepearl/privacy.html) · [support](./musepearl/support.html) |
| `ohkeys/` | Oh Keys - LLM Balance（大模型余额助手） | [privacy](./ohkeys/privacy.html) · [support](./ohkeys/support.html) |

## Usage / 用途

这些页面的公网 URL 用于 App Store Connect / Google Play 的 **Privacy Policy URL** 与 **Support URL**。

Base URL: `https://<username>.github.io/legal-pages/`

## Notes / 说明

- 仅存放**对外公开**的法律与支持页面；**不含**任何源码、密钥或用户数据。
- 内容源与项目文档保持同步；隐私政策须与 App 实际行为、商店隐私标签一致。


## 维护关系 / Maintenance model

这里不是三份独立的隐私政策，而是一条“本地 Git 工作副本 → GitHub 远端仓库 → GitHub Pages 公网页面”的发布链：

- `/Users/xiaojun/projects/legal-pages/`：本地版本管理、编辑、历史追溯和发布前验证工作副本。
- `wdxdd/legal-pages`：远端备份与 GitHub Pages 的发布来源；推送必须由用户明确确认。
- `legal-pages/<project>/`：仓库内部的项目子目录，用于隔离多个项目的 `index.html`、`privacy.html` 和 `support.html`，不是额外仓库，也不是另一份需要独立维护的政策。
- `https://wdxdd.github.io/legal-pages/<project>/privacy.html`：最终对外公开 URL，用于 App Store Connect / Google Play 等平台。

跨项目职责、项目登记、语言阶段、版本和验证规则统一见 [`APP隐私政策统一管理规范`](../00-project-manage/APP隐私政策统一管理规范.md)。
