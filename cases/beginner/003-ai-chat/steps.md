# Case 003 · Steps（步骤）

## Step 1 · 准备环境

1. 安装 Node.js（以 [官方文档](https://nodejs.org/) 为准，选 LTS 版本）
2. 确认安装成功：终端运行 `node -v`
3. 注册并获取 AI API 账号和 Key（以服务商文档为准）

## Step 2 · 创建项目骨架

新建文件夹 `ai-chat`，用 AI 工具打开。让 AI 创建前后端文件结构（见 [start.md](prompts/start.md) 的第一步）。

## Step 3 · 配置环境变量

创建 `.env` 文件（**确保它在 .gitignore 里**），放入你的 Key：

```text
API_KEY=你的真实Key
```

> 永远不要提交 `.env` 文件。如果误提交，立即撤销 Key 并重新生成。

## Step 4 · 让 AI 实现后端转发

用 [start.md](prompts/start.md) 的 Prompt，让 AI 实现：后端接收前端消息 → 调用 AI API → 返回回答。

## Step 5 · 让 AI 实现前端界面

实现输入框、对话区、加载状态和错误提示。

## Step 6 · 运行和验证

按 [verification.md](verification.md) 验证。遇到错误用 [debug.md](prompts/debug.md)。

## Step 7 · 记录

完成验证表，读 [lessons.md](lessons.md)。

## 完成标准

- [ ] 完成一轮 AI 对话
- [ ] 有加载状态和错误提示
- [ ] Key 只存在于环境变量
- [ ] 本地运行无报错
