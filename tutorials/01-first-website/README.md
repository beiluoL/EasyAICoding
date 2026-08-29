# Tutorial 01 · 第一个网页

## 你要做什么

用 AI 做一个展示你自己的网页，只有几个文件，任何电脑都能打开。

## 最终会得到什么

一个能双击打开的 `index.html`：显示你的名字、介绍、按钮，按钮点击后有反馈。

## 准备工作

- 一个 AI 工具（[不知道怎么选？](../../docs/getting-started/03-choose-your-ai-tool.md)）
- 一个文件夹，例如桌面 `my-website`
- 约 30-60 分钟

## Step 1 · 创建项目文件夹

在桌面新建文件夹，命名为 `my-website`。

> 为什么要文件夹？项目文件集中管理，AI 和你都容易理解。[Project（项目）](../../docs/concepts/project.md)

## Step 2 · 让 AI 生成网页

打开 AI 工具，复制 [prompts.md](prompts.md) 里的「开始 Prompt」，把 `{{你的名字}}` 和 `{{你的介绍}}` 替换成真实信息，发送。

## Step 3 · 保存文件

在 `my-website` 里新建文件 `index.html`，把 AI 给的完整代码粘贴进去，保存。

⚠️ 注意：文件名必须是 `index.html`，不是 `index.html.txt`。

## Step 4 · 运行

双击 `index.html`，或把它拖进浏览器。

**预期看到**：页面显示你的名字、介绍、按钮，页面不是空白。

## Step 5 · 验证按钮

点击按钮。

**预期看到**：出现一条欢迎消息。

如果没反应，打开浏览器开发者工具（按 F12），看 Console 有没有红色错误，把错误发给 AI。

## Step 6 · 修改你的网站

让 AI 帮你修改：

```text
请把 index.html 的背景色改成浅蓝色，按钮改成圆角，其他不要动。
```

保存 → 刷新 → 验证。

## Step 7 · 完成记录

读一下 [Case 001 的经验教训](../../cases/beginner/001-personal-website/lessons.md)，写下你学到的 3 件事。

## 运行

任何时候，双击 `index.html` 或用浏览器打开它即可。

## 常见错误

| 现象 | 原因 | 解决 |
| --- | --- | --- |
| 双击打不开 | 文件名带了 `.txt` | 重命名为 `index.html` |
| 页面空白 | 代码没保存或复制不完整 | 重新复制完整代码保存，确认末尾有 `</html>` |
| 按钮没反应 | JavaScript 报错 | F12 看 Console，把错误发给 AI |
| 页面难看 | CSS 没生效 | 检查 `<link>` 引入的 CSS 路径 |

## 下一步

- 继续美化你的网站（配色、照片、多个按钮）
- 学习 [Tutorial 03 · Todo 应用](../03-first-todo-app/README.md)
- 或者先看 [什么是 Vibe Coding](../../docs/getting-started/02-what-is-vibe-coding.md)

## Verification

- 本教程的步骤与 [Case 001](../../cases/beginner/001-personal-website/README.md) 一致，基于通用实践整理
- Verification: Not Yet Verified
