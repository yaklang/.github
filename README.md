<div align="center">

<img src="profile/assets/yak-logo.png" alt="YAK" width="280" />

# `.github` · Yaklang.io 组织元仓库

<em>Organization-level meta repository for <a href="https://github.com/yaklang">@yaklang</a></em>

</div>

---

## 这是什么 · What is this

这是 GitHub 为「组织」准备的特殊仓库。它**不放产品代码**，只承载整个 [@yaklang](https://github.com/yaklang) 组织共享的「门面」与「默认配置」。

最重要的文件是 [`profile/README.md`](profile/README.md) —— 它会被 GitHub 直接渲染成组织主页 <https://github.com/yaklang> 顶部的简介（BIO）。

> *A special GitHub repository whose `profile/README.md` is rendered as the public profile of the entire organization.*

## 目录结构 · Layout

```
.github/
├── README.md            # 本文件：仓库自身说明（仅在本仓库页面可见）
└── profile/
    ├── README.md        # 组织主页 BIO（渲染在 github.com/yaklang 顶部）
    └── assets/          # BIO 用到的图片（Hero / LOGO / 图标）
        ├── hero.png
        ├── yak-logo.png
        └── yak-icon.png
```

## 如何更新组织主页 · How to update the org profile

1. 编辑 [`profile/README.md`](profile/README.md)，图片放进 `profile/assets/`，用相对路径 `assets/xxx.png` 引用。
2. 提交并推送到默认分支。
3. 刷新 <https://github.com/yaklang> 即可看到更新（通常即时生效）。

## `.github` 仓库还能做什么 · What else this repo can do

除了组织主页，这个仓库还能集中托管「组织级默认资源」。任何成员仓库若**自身没有**对应文件，就会**回退继承**这里的版本，从而做到一处维护、全组织生效：

| 能力 | 放置路径 | 作用 |
| :--- | :--- | :--- |
| 组织主页 BIO | `profile/README.md` | 渲染为组织主页简介（本仓库核心用途） |
| 默认 Issue 模板 | `.github/ISSUE_TEMPLATE/*.md` / `*.yml` | 全组织仓库共享的 Bug / Feature 提报模板 |
| Issue 模板配置 | `.github/ISSUE_TEMPLATE/config.yml` | 关闭空白 issue、引导到文档 / 社区入口 |
| 默认 PR 模板 | `.github/PULL_REQUEST_TEMPLATE.md` | 统一 PR 描述结构与自查清单 |
| 贡献指南 | `CONTRIBUTING.md` | 全组织默认贡献规范 |
| 行为准则 | `CODE_OF_CONDUCT.md` | 社区行为准则 |
| 安全策略 | `SECURITY.md` | 漏洞披露流程与联系方式（安全团队尤其重要） |
| 资助入口 | `FUNDING.yml` | 仓库页面的 Sponsor 按钮配置 |
| 支持入口 | `SUPPORT.md` | 引导用户到正确的求助渠道 |
| 复用型工作流 | `workflow-templates/` | 组织内可一键复用的 GitHub Actions 模板 |
| 默认讨论/通知 | `.github/` 下相关配置 | 组织层面的默认协作配置 |

> 继承规则：成员仓库优先使用**自己仓库内**的同名文件；只有缺失时才回退到 `.github` 仓库的版本。因此可以在这里维护一套「组织默认」，再让个别仓库按需覆盖。

## 相关站点 · Sites

[yaklang.com](https://yaklang.com) · [memfit.ai](https://memfit.ai) · [ssa.to](https://ssa.to) · [rag.yaklang.com](https://rag.yaklang.com) · [skills.yaklang.io](https://skills.yaklang.io) · [hackbenchmark.com](https://hackbenchmark.com)

<div align="center">
<sub>做难而正确的事 · Do the hard, right things. — © Yaklang.io Project</sub>
</div>
