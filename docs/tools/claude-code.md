# Claude Code

> 重要提示：本指南为方向性说明，安装与最新操作请以 [Anthropic Claude Code 官方文档](https://docs.anthropic.com/en/docs/claude-code/overview) 为准。

## 它是什么？

Claude Code 是 Anthropic 推出的终端 AI 编程工具。你在终端里用自然语言和 Claude 对话，它可以读取项目文件、修改代码、运行命令。

## 适合谁？

- 能接受使用终端（Terminal）的人
- 喜欢文字界面、关注输出细节的人
- 用 Claude 模型做开发的人

## 怎么安装？

1. 打开官方文档，确认当前安装方式（通常通过命令行安装）
2. 安装后确认版本命令可用
3. 首次使用需要登录或配置 API Key

> 不要把 API Key 写进任何会被提交的文件。

## 第一次怎么使用？

1. 新建项目文件夹：`mkdir my-website && cd my-website`
2. 在文件夹内启动 Claude Code
3. 从 [start-project Prompt](../../prompts/start/start-project.md) 开始对话

## 怎么让 AI 理解项目？

- 在项目根目录启动，让它直接读取文件
- 项目内维护 `README.md` 和清晰的目录结构
- 对话太长或开新会话时，重新交代背景（[Context（上下文）](../concepts/context.md)）

## 怎么让 AI 修改代码？

具体说明文件路径和改动内容，参考 [modify-code Prompt](../../prompts/coding/modify-code.md)。

## 怎么 Debug？

1. 在项目里运行，复现错误
2. 复制完整错误信息给 Claude Code
3. 使用 [debug-error Prompt](../../prompts/debugging/debug-error.md)

## 优点 / 注意

- 优点：文本输出清晰、适合逐步推进、可以执行命令验证
- 注意：终端操作需要一点基本概念（当前目录、运行命令），遇到不懂的术语直接问它

## Verification

- 本文件为通用指南
- Verification: Not Yet Verified（请以官方文档为准）
