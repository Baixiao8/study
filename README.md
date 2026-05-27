# 学习思考 · Study & Thinking 〈已退役〉

> 本仓库的所有项目已合并到 **[studies · 深度研究档案](https://baixiao8.github.io/studies/)** 统一管理。
> 合并日期:2026-05-27 · 此仓库保留作为存档,所有 index.html 已改为跳转页。

---

## 迁移对照表

| 原项目 | 新位置 | 分区 |
|---|---|---|
| marathon | [studies/reports/2026-05-marathon/](https://baixiao8.github.io/studies/reports/2026-05-marathon/) | I · 运动科学 |
| thinking-evolution | [studies/reports/2026-05-thinking-evolution/](https://baixiao8.github.io/studies/reports/2026-05-thinking-evolution/) | II · UX & 产品 |
| anthropic-academy | [studies/reports/2026-05-anthropic-academy/](https://baixiao8.github.io/studies/reports/2026-05-anthropic-academy/) | III · AI 工程 |
| skills-building-guide | [studies/reports/2026-05-skills-building-guide/](https://baixiao8.github.io/studies/reports/2026-05-skills-building-guide/) | III · AI 工程 |

---

## 为什么要合并

两个仓库 `study`(学习笔记)+ `studies`(深度研究档案)定位过近,用户记不清入口,marathon 出现过错位(studies 首页有卡片但实体在 study)。

合并后只剩 studies 一个入口,按 I / II / III 分区组织,边界硬化:

- **新报告**(长篇深度调研、单页 SPA 笔记、资料库)→ 全部进 studies/reports/YYYY-MM-<slug>/
- 长篇深度调研走 A 模式(parts/+chapters/ + CI 装配)
- 单页 SPA / 资料库走 B 模式(整目录由 CI mirror,见 [studies workflow](https://github.com/Baixiao8/studies/blob/main/.github/workflows/build-and-deploy.yml))

---

## 历史

| 版本 | 日期 | 内容 |
|---|---|---|
| v0 → 退役 | 2026-05-27 | 4 个子项目迁入 studies,本仓库 index.html 全部改跳转 |
| v0.1 | 2026-05-27 | 补全所有项目的 GitHub Pages 在线链接 |
| v0 | 2026-05-21 | 仓库初建,marathon v4 等项目陆续加入 |

完整的 commit 历史可以 `git log` 查看。

---

*Last updated: 2026-05-27 · 仓库退役 · 项目全部迁往 [studies](https://baixiao8.github.io/studies/)*
