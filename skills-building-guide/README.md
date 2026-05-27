# Skills Building Guide · 中文化学习笔记

> Anthropic 官方《The Complete Guide to Building Skills for Claude》的中文重写版本。
> **不是直译**——用中文重新组织，加入类比和例子，专业名词保留英文 + 中文注释。

- **当前版本**：v0.1
- **最近更新**：2026-05-27
- **入口**：[index.html](./index.html)

---

## 这个项目是什么

把英文版 33 页指南转成"我能真正读懂"的中文学习笔记。

设计风格沿用「运动健康」项目的 newsprint 报纸版式（泛黄纸张 / Inter Tight 大标题 / 朱砂红强调），针对教程体裁做了适配——保留代码块、增加章首 TOC、关键步骤显式编号。

## 文件结构

```
skills-building-guide/
├── README.md         # 本文件
├── CHANGELOG.md      # 版本演进
├── source.pdf        # 原始英文 PDF（33 页）
├── index.html        # 首页索引 · 报头 + Introduction + 7 章导航
├── ch1-fundamentals.html         # 第 1 章 · 基础概念
├── ch2-planning-design.html      # 第 2 章 · 规划与设计（待完成）
├── ch3-testing-iteration.html    # 第 3 章 · 测试与迭代（待完成）
├── ch4-distribution-sharing.html # 第 4 章 · 分发与分享（待完成）
├── ch5-patterns-troubleshooting.html # 第 5 章 · 模式与排错（待完成）
└── ch6-resources-references.html # 第 6 章 · 资源与参考（待完成）
```

## 本地预览

```bash
cd ~/白笑/claude/报告库/学习思考/skills-building-guide
python3 -m http.server 8765
# 浏览器打开 http://127.0.0.1:8765/
```

也可以直接在 Finder 里双击 `index.html`——所有样式内联、不依赖后端。

## 接下来要做什么

- 完成 ch2 ~ ch6 五章的中文重写
- 三个附录（Quick checklist / YAML frontmatter / Complete skill examples）合并到 ch6
- 全部完成后打 v1.0
