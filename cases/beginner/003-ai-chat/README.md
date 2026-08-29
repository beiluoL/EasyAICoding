# Case 003 · AI 聊天

## 项目是什么

做一个简单的 AI 聊天网页：用户输入文字，调用 AI API 返回回答，对话显示在页面上。

## 适合谁

- 完成 [Case 001](../001-personal-website/README.md) 和 [Case 002](../002-todo-app/README.md) 的人
- 第一次调用 AI API（接口）的人

## 难度

⭐⭐⭐

## 学习目标

- 理解 API（接口）的基本概念：请求（Request）和响应（Response）
- 理解为什么 API Key 不能写进前端代码
- 学会通过后端转发 AI API 请求
- 学会处理加载状态和错误

## 需要什么

- 一个 AI 工具
- 一个 AI API 账号（OpenAI、Anthropic、国内大模型等，以官方文档为准）
- Node.js 环境（用于跑后端，安装见 [环境问题](../../../debugging/environment/README.md)）
- 约 2-3 小时

## 最终效果

本地运行后，浏览器打开页面：输入问题 → 点击发送 → 等待几秒 → 看到 AI 的回答。

## 重要安全说明

**API Key 只放在后端的环境变量里，绝不放进前端代码，绝不提交到 GitHub。**

## 相关链接

- [步骤](steps.md)
- [需求](requirements.md)
- [Prompt](prompts/start.md)
- [验证](verification.md)
- [经验教训](lessons.md)
- [教程 02](../../../tutorials/02-first-ai-chat/README.md)

## Verification

- Verification: Not Yet Verified
