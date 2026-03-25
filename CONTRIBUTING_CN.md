# 贡献指南

感谢你对本项目的关注！以下是参与贡献的简要说明，请在提交 PR 之前阅读。

---

## 分支管理

- **`master` 为保护分支**，禁止直接推送，所有改动必须通过 Pull Request 提交。
- 从 `master` 创建你的分支，命名清晰：
  - `add/glossary-trade` — 新增内容
  - `fix/sql-tutorial-typo` — 修复问题
  - `update/standards-naming` — 更新已有内容
- 每个 PR 至少需要 **1 位维护者审核** 通过后才能合并。
- 合并时使用 **Squash and Merge**，保持提交历史整洁。

## 目录结构

```
data-warehouse/
├── index.html              ← 站点首页（新增模块时需同步更新）
├── assets/style.css        ← 公共样式（不要在子目录中重复定义）
├── sql-tutorial/           ← SQL 练习平台
├── standards/              ← 数仓规范
├── glossary/               ← 命名词根字典
└── docs/                   ← 项目文档（非面向用户的内容）
```

## 命名规范

| 类型 | 规则 | 示例 |
|------|------|------|
| 目录名 | 全小写，用 `-` 连接 | `sql-tutorial/` |
| HTML 文件 | 全小写，多词用 `_` 连接 | `sql_practice.html` |
| CSS / JS 文件 | 全小写，用 `-` 连接 | `style.css` |
| 分支名 | `类型/简短描述` | `add/glossary-finance` |

## 如何新增内容

1. **先提 Issue** — 简要描述你想添加的内容，让维护者确认方向后再动手。
2. 如果目录不存在，创建对应目录。
3. HTML 文件必须引用公共样式表：
   ```html
   <link rel="stylesheet" href="../assets/style.css">
   ```
4. 页面风格保持深色主题统一，使用 `assets/style.css` 中定义的 CSS 变量。详见 [风格指南](docs/style-guide.md)。
5. 在 `index.html` 首页中为新模块添加入口卡片。
6. 按照 PR 模板提交 Pull Request。

## Commit 格式

简短清晰，使用前缀：

```
add: 窗口函数练习题
fix: 词根字典页面断链
update: 命名规范章节
docs: 完善贡献指南
```

## 审核清单

PR 审核时，维护者会检查以下内容：

- [ ] 分支基于最新 `master`
- [ ] 内容准确、表述清晰
- [ ] HTML 遵循公共样式（深色主题、一致的布局）
- [ ] 无断链、无缺失资源
- [ ] 新增模块时已更新 `index.html` 首页
- [ ] Commit 信息规范

## 有问题？

提一个带 **Question** 标签的 Issue，我们很乐意帮忙！
