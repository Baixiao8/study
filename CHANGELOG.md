# Changelog · 学习思考

> 仓库级演进记录。每个子项目（如 `marathon/`）有自己独立的 CHANGELOG。
> 版本号规则见 [../CONVENTIONS.md](../CONVENTIONS.md)。

---

## 2026-05-27 · 新增 skills-building-guide 子项目（v0.1 → v0.3）

### 新增：Skills 构建指南中文化对照本

- 新建 [`skills-building-guide/`](./skills-building-guide/)，对 Anthropic 官方 33 页《The Complete Guide to Building Skills for Claude》做中文化
- 设计风格沿用「运动健康」项目的 newsprint 报纸版式，针对教程体裁做了适配

### 迭代历程（同日三个版本）

- **v0.1**：首页 + 第 1 章样本，B 路线（中文重写）
- **v0.2**：风格切换到 C 路线（英文原句保留 + 中文导读对照），首页和第 1 章返工
- **v0.3**：合并为单文件 SPA + hash 路由（点章节卡新开标签页），全 6 章 + 3 附录补齐

---

## 2026-05-21 · 结构升级

### 重构：marathon 子项目升级到完整结构

参考 `miniapps/Tech Words` 的成熟模式，把 marathon 子项目重组为：

```
marathon/
├── README.md / ARCHITECTURE.md / CHANGELOG.md / 项目文档.md
├── index.html（GitHub Pages 入口）
├── images/ archive/ generation/ knowledge/ memory/
```

marathon 当前版本 v4，详细演进见 [marathon/CHANGELOG.md](./marathon/CHANGELOG.md)。

### 下一步

后续每个新加入的学习项目（一个主题一个独立子目录）都按这一套结构搭。
