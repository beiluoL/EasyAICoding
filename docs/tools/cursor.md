# Cursor

> 重要提示：本指南为方向性说明，安装与最新操作请以 [Cursor 官方文档](https://docs.cursor.com/) 为准。

## 它是什么？

Cursor 是一个带 AI 的代码编辑器，界面和 VS Code 很相似。你可以在里面打开项目文件夹，像聊天一样让 AI 帮你写代码、改代码、解释代码。

## 适合谁？

- 不想用命令行、喜欢可视化界面的人
- 想一边看代码一边和 AI 对话的人
- 从零开始学习编程的人（编辑器自带补全和提示，帮助理解）

## 怎么安装？

1. 打开官方下载页面，下载对应操作系统（macOS / Windows / Linux）的安装包
2. 像安装普通软件一样安装
3. 打开后登录账号

## 第一次怎么使用？

1. 菜单选择「打开文件夹」（Open Folder），打开你的项目文件夹（或新建一个）
2. 在 AI 对话面板（Chat / Composer）里开始对话
3. 从 [start-project Prompt](../../prompts/start/start-project.md) 开始

## 怎么让 AI 理解项目？

- 打开整个项目文件夹，Cursor 可以读取项目文件
- 使用 @ 功能引用具体文件（例如 `@index.html`），让 AI 聚焦在某个文件上
- 在项目里维护 `README.md`

## 怎么让 AI 修改代码？

在对话里明确说：改哪个文件、怎么改。Cursor 会给出修改建议，你可以直接接受（Accept）或拒绝。

示例：

```text
把 index.html 的标题改成「我的第一个网站」。
```

## 怎么 Debug？

1. 运行项目复现错误
2. 选中错误信息或相关代码，粘贴到对话里
3. 使用 [debug-error Prompt](../../prompts/debugging/debug-error.md)

## 优点 / 注意

- 优点：可视化、上手快、可以一边看文件一边对话
- 注意：编辑器功能很多，新手先只用「打开文件夹 + 对话」两个功能就够了，其他以后慢慢学

## Verification

- 本文件为通用指南
- Verification: Not Yet Verified（请以官方文档为准）
