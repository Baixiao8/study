# Anthropic Academy 学院全景笔记 · 早期导览版(已弃用)

> ⚠️ **这是早期的导览本版本,已被深度调研版本取代。**
>
> 完整深度版(15 章 · 80K 字 · 3.8h 阅读)在 studies 仓:
> 👉 **[Anthropic 与 Claude 深度调研](https://baixiao8.github.io/studies/reports/2026-05-anthropic-academy/)**
>
> 深度版从「LLM 是什么」零基础讲起,15 章覆盖 LLM 原理 / 4D 方法论 / 产品全家桶 / Claude Code 工程 / MCP 协议 / Agent 架构 / 18 门课速查与角色路径。

---

## 早期导览版说明

- **当前版本**:v0.1(已冻结,不再迭代)
- **入口**:[index.html](./index.html)(轻量版,18 门课速查 + 5 角色路径,60-90 分钟读完)
- **课程源**:https://anthropic.skilljar.com/(免费、官方证书)
- **覆盖课程**:18 门(截至 2026-05)
- **跟深度版的区别**:导览本是「课程菜单 + 选课指南」(12K 字);深度版是「能直接学到 LLM 核心知识的书」(80K 字)。新读者建议直接看深度版。

---

## 这个项目是什么

Anthropic 在 2026 年 3 月开了官方学习平台 [Skilljar Academy](https://anthropic.skilljar.com/),上面有 18 门课,全免费、带官方证书。**问题是——总时长超过 22 小时,内容横跨 5 个轨道**,不是每门都值得花时间。

这份笔记的目标:**让你不必逐门上课,也能拿到这 18 门课的精华**。

- 知道每门课讲什么(30 秒精华卡)
- 知道每门课该不该花时间(尖锐判断 + 跳过条件)
- 知道按你的角色应该走哪条学习路径
- 把课程里最值得带走的概念,用中文重新讲一遍

风格上沿用「[Skills 构建指南](../skills-building-guide/)」的 newsprint 报纸版式(米黄纸张 / Inter Tight 大标题 / 朱砂红强调),做成单文件 SPA + hash 路由,点章节卡新开标签页。

## 内容覆盖

| Hash | 板块 | 主题 |
|---|---|---|
| `#home` | 首页 | 全景介绍 + 数据带 + 5 大轨道入口 + 18 门课速查表 + 我该学哪门(决策器) |
| `#t1` | 轨道一 · 入门基础 | Claude 101、AI Capabilities and Limitations |
| `#t2` | 轨道二 · AI 素养(4D 框架) | Framework & Foundations + 5 门面向不同人群的版本 |
| `#t3` | 轨道三 · 开发者深度 | Claude Code 101/in Action、Agent Skills、Subagents、Cowork |
| `#t4` | 轨道四 · API 与协议 | Building with Claude API、MCP Intro/Advanced |
| `#t5` | 轨道五 · 云平台部署 | Amazon Bedrock、Google Cloud Vertex AI |
| `#core` | 精华提炼 | 6 个贯穿所有课的核心概念(自己消化版) |
| `#paths` | 学习路径 | 按 5 种角色给出最优路径(开发者 / 产品 / 教育 / 业务 / 决策者) |
| `#glossary` | 术语速查 | 25 个高频术语中英对照 |

## 18 门课全景

```
[Foundation 入门]                          [Build 进阶]
├─ Claude 101                              ├─ Claude Code 101
└─ AI Capabilities and Limitations         ├─ Claude Code in Action
                                           ├─ Introduction to Agent Skills
[AI Fluency 素养 · 6 门]                   ├─ Introduction to Subagents
├─ AI Fluency: Framework & Foundations     └─ Introduction to Claude Cowork
├─ AI Fluency for Educators
├─ AI Fluency for Students                 [API & Protocol]
├─ AI Fluency for Nonprofits               ├─ Building with the Claude API ★ 8.1h
├─ AI Fluency for Small Businesses         ├─ Introduction to MCP
└─ Teaching AI Fluency                     └─ MCP: Advanced Topics

[Cloud 云部署]
├─ Claude with Amazon Bedrock
└─ Claude with Google Cloud Vertex AI
```

## 文件结构

```
anthropic-academy/
├── README.md         # 本文件
├── CHANGELOG.md      # 版本演进
├── 项目文档.md       # 项目状态、关键决策
├── index.html        # 单文件 SPA(首页 + 5 轨道 + core/paths/glossary)
└── archive/          # 历史版本备份
```

## 本地预览

```bash
cd ~/白笑/claude/报告库/学习思考/anthropic-academy
python3 -m http.server 8765
# 打开 http://127.0.0.1:8765/
```

也可以直接 Finder 双击 `index.html`——样式内联、不依赖后端。

## 数据来源

- 课程结构、模块、课时:Anthropic Skilljar 官方页面(每门课 URL 见首页课表)
- 4D 框架定义:Prof. Joseph Feller + Prof. Rick Dakan(Anthropic 学术合作)
- 时长 / 课时数 / 测验数:Skilljar 课程页面 + 第三方汇总博客交叉验证
- 我的判断、跳过条件、学习路径:基于课程定位 + 用户角色分析

## 接下来要做什么

- v0.1 完成 18 门课全景 + 5 轨道精华卡 + 核心知识提炼
- 后续可能:
  - 等 Anthropic 出新课后做差异更新
  - 加每门课实际跑完的体感笔记(已选学完的)
  - 把 4D 框架做成可交互的决策器
