# Tutorial 03 · 第一个 Todo 应用

## 你要做什么

做一个待办清单应用：添加任务、标记完成、删除任务，最后部署上线让别人能用。

## 最终会得到什么

一个本地可用的 Todo 应用 + 一个公网链接（部署后）。

## 准备工作

- 完成 [Tutorial 01](../01-first-website/README.md)
- 一个 AI 工具
- 一个 GitHub 账号（用于部署，可选但推荐）
- 约 1-2 小时（部署再加 1 小时）

## Step 1 · 创建项目

新建文件夹 `todo-app`，用 AI 工具打开。

## Step 2 · 生成 MVP

复制 [prompts.md](prompts.md) 的「开始 Prompt」发给 AI。

## Step 3 · 运行验证

双击 `index.html` 或启动本地服务。

验证五项核心功能：

1. 添加任务
2. 任务出现在列表
3. 点击标记完成
4. 删除任务
5. 空列表有提示

## Step 4 · 加统计功能

让 AI 加「已完成 X / 共 Y」和「清空已完成」按钮（用 [prompts.md](prompts.md) 的修改 Prompt）。

## Step 5 · Debug 练习

故意制造一个错误：

```text
请把 script.js 里绑定添加按钮的那行代码改错（比如 id 写错），然后告诉我。
```

运行看到报错后，用 Debug Prompt 修复。这能让你亲身体验 Debug 流程。

## Step 6 · 部署上线

把项目推到 GitHub，然后用 GitHub Pages 部署（静态项目最简单的方式）。

用这个 Prompt 让 AI 一步步带你做：

```text
我想把 todo-app 部署到 GitHub Pages。请一步步教我：
1. 如何在 GitHub 创建仓库并推送代码
2. 如何开启 GitHub Pages
3. 每一步告诉我「预期看到什么」
```

## 运行

本地：双击 `index.html`，或 `npx serve .` 启动本地服务。

## 常见错误

| 现象 | 原因 | 解决 |
| --- | --- | --- |
| 添加没反应 | id 不匹配或 JS 没引入 | 检查 HTML 是否引入了 script.js |
| 点击不切换完成 | 动态元素事件绑定问题 | 让 AI 用事件委托实现 |
| 部署后白屏 | 路径问题 | 检查资源路径，让 AI 修复 |
| 数据刷新就没了 | 还没做持久化 | 这是当前版本的预期行为 |

## 下一步

- 让 AI 加 localStorage，实现刷新不丢数据（很实用的练习）
- 做 [Tutorial 02 · AI 聊天](../02-first-ai-chat/README.md)（如果还没做）
- 完整案例见 [Case 002](../../cases/beginner/002-todo-app/README.md)

## Verification

- 本教程与 [Case 002](../../cases/beginner/002-todo-app/README.md) 基于同一方案
- Verification: Not Yet Verified（部署步骤以 GitHub 官方文档为准）
