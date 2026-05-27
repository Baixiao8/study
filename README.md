# 学习思考 · Study & Thinking

个人学习沉淀仓库 —— 收纳系统性学习成果,以可分享的形式（HTML / Markdown / Notebook）发布。

> 在线主页:https://baixiao8.github.io/study/

---

## 项目列表

| 项目 | 类型 | 在线链接 | 文档 | 当前版本 |
|---|---|---|---|---|
| 运动科学手册 | HTML 技术手册 + 视觉化 | [打开 →](https://baixiao8.github.io/study/marathon/) | [marathon/README.md](./marathon/README.md) | v4 |
| 思考进化 | Bento Box 单页 + UX 资料库 | [打开 →](https://baixiao8.github.io/study/thinking-evolution/) | [thinking-evolution/README.md](./thinking-evolution/README.md) | v0.1 |
| Skills 构建指南（中文化笔记） | Newsprint 风格 HTML 学习笔记 | — | [skills-building-guide/README.md](./skills-building-guide/README.md) | v0.3 |
| Anthropic Academy 全景笔记 | Newsprint 风格 18 门课导览 | — | [anthropic-academy/README.md](./anthropic-academy/README.md) | v0.1 |

后续会陆续加入其他学习项目,每个一个独立子目录,配独立的可分享短链。

---

## 仓库治理

每个项目子目录都采用同一套结构（参考 [`miniapps/Tech Words`](https://github.com/Baixiao8) 的成熟模式）:

```
<project>/
├── README.md              ← 项目说明 + 线上链接 + 核心摘要
├── ARCHITECTURE.md        ← 内容架构 + 视觉系统 + 命名约定
├── CHANGELOG.md           ← 版本迭代史
├── 项目文档.md             ← 项目状态、关键决策、待办
├── index.html             ← GitHub Pages 入口
├── images/                ← 资源
├── archive/               ← 历史版本备份
├── generation/            ← 生成工具链(scripts + prompts)
├── knowledge/             ← 知识库(分类目录 + README 索引)
└── memory/                ← Agent 记忆(MEMORY.md + project_*.md)
```

### 添加新项目的工作流

```bash
cd ~/白笑/claude/学习思考
mkdir 新项目目录/   # 用英文短名,如 coding/、design/
# 在里面建上述结构 + index.html
git add . && git commit -m "add: 新项目" && git push
# GitHub Pages 30-60 秒自动部署
# 新链接: https://baixiao8.github.io/study/新项目目录/
```

### 维护规则

- 每次大改动:**先备份当前 `index.html` 到 `archive/manual-vX.html`**,再改
- 改动后更新 `CHANGELOG.md` 顶部
- 内容铁律写进 `ARCHITECTURE.md`,新增功能前对照检查
- AI 生成图 prompt 用 text-safe 模板（参考 `<project>/generation/prompts/hero_v3.py`）

---

*Last updated: 2026-05-27 · 新增 anthropic-academy v0.1*
