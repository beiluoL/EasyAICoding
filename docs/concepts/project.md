# Project（项目）

## 定义

**Project（项目）**：为了实现一个软件目标而组织起来的一组文件和配置。

大白话：**项目就是一个「软件的文件夹」。** 里面装着代码、说明和资源，这些文件合在一起构成了你的软件。

## 例子

一个最简单的个人网站项目：

```text
my-website/
├── index.html    # 网页内容
├── style.css     # 网页样式（可选）
├── script.js     # 网页交互（可选）
└── README.md     # 项目说明（可选但推荐）
```

## 为什么要把东西放进「项目」里

1. **AI 更容易理解**：打开项目文件夹，AI 能看到全部文件，而不是靠猜
2. **不容易丢**：所有文件集中在一个文件夹，备份、压缩、迁移都方便
3. **可以分享**：整个文件夹分享出去，别人也能运行

## 新手容易犯的错

### 错误 1：所有文件乱放在桌面

❌ 桌面一堆 `index.html`、`新建文档(3).html`

✅ 每个项目一个文件夹，名字有意义：`my-website`、`todo-app`

### 错误 2：项目文件夹里塞满无关文件

保持项目干净。下载的安装包、临时截图放别处。

### 错误 3：项目没有说明

在项目里放一个 `README.md`，写清楚：这是什么、怎么运行。这对自己和 AI 都有帮助。

## 什么是「让 AI 理解项目」

让 AI 理解项目 = 让 AI 能看到你的项目文件和结构。常见方式：

- 用支持打开文件夹的工具（Cursor、Codex 等）
- 把关键文件内容贴给 AI
- 提供 [requirements（需求）和 README](../../templates/requirement.md)

## 相关

- [Context（上下文）](context.md)
- [Frontend（前端）](frontend.md)
- [Backend（后端）](backend.md)

## Verification

- 内容类型：概念解释
- Verification: Not Yet Verified
