# Codex

> 重要提示：本指南为方向性说明，安装与最新操作请以 [OpenAI Codex 官方文档](https://developers.openai.com/codex/) 为准。

## 它是什么？

Codex 是 OpenAI 提供的 AI Coding 工具，可以理解为「住在终端或桌面 App 里的编程搭档」。你用自然语言和它对话，它帮你创建、修改、运行、调试代码。

## 适合谁？

- 想要「对话式」从零构建项目的人
- 能接受打开终端（Terminal）或使用桌面 App 的人
- 想做一个完整项目（而不只是改几个文件）的人

## 怎么安装？

1. 打开官方文档，找到当前推荐的安装方式
2. 按操作系统（macOS / Windows / Linux）选择对应方法
3. 安装后运行 `codex --version`（或在桌面 App 中查看版本），确认安装成功
4. 首次使用需要登录账号

## 第一次怎么使用？

1. 新建一个文件夹作为项目，例如 `my-website`
2. 在终端进入该文件夹：`cd my-website`
3. 启动 Codex，开始对话
4. 从 [start-project Prompt](../../prompts/start/start-project.md) 开始

## 怎么让 AI 理解项目？

- 在项目文件夹内启动，让 Codex 直接读取项目文件
- 新会话开始时，用一句话说明项目背景（[Context（上下文）](../concepts/context.md)）
- 在项目里放好 `README.md`，说明项目是什么、怎么运行

## 怎么让 AI 修改代码？

明确告诉它：改哪个文件、改成什么、不要动什么。参考 [modify-code Prompt](../../prompts/coding/modify-code.md)。

示例：

```text
打开 index.html，把背景颜色改成浅蓝色，其他内容不要动。
```

## 怎么 Debug？

1. 运行你的项目
2. 把完整的错误信息 + 现象发给 Codex
3. 使用 [debug-error Prompt](../../prompts/debugging/debug-error.md)

## 优点 / 注意

- 优点：适合项目级对话、能连续构建、能执行命令
- 注意：它按你的指令做事，需求说得越清楚，结果越接近预期

## Verification

- 本文件为通用指南
- Verification: Not Yet Verified（请以官方文档为准）
