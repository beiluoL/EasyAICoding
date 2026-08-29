# Tutorial 02 · 第一个 AI 聊天

## 你要做什么

做一个 AI 聊天网页：输入问题，AI 回答，对话显示在页面上。

## 最终会得到什么

一个本地运行的小应用：前端页面 + 后端服务，后端负责安全地调用 AI API。

## 准备工作

- 完成 [Tutorial 01](../01-first-website/README.md)
- 一个 AI API 账号（OpenAI / Anthropic / 国内大模型，以官方文档为准）
- 安装 Node.js（[官方文档](https://nodejs.org/) 选 LTS，装完终端运行 `node -v` 验证）
- 约 2-3 小时

## Step 1 · 理解结构

这个项目有两个部分：

```text
前端（public/）→ 你看到的聊天界面
后端（server.js）→ 偷偷调用 AI API 的「中间人」
```

为什么需要后端？因为 API Key 放在前端会被任何人看到。[Backend（后端）](../../docs/concepts/backend.md)

## Step 2 · 创建项目

新建文件夹 `ai-chat`，用 AI 工具打开。复制 [prompts.md](prompts.md) 的「创建结构」Prompt 发给 AI。

## Step 3 · 配置 API Key

1. 创建 `.env` 文件
2. 放入：`API_KEY=你的真实Key`
3. 确认 `.gitignore` 里包含 `.env`

⚠️ `.env` 一旦被提交到 GitHub，立即去服务商后台撤销这个 Key 并重新生成。

## Step 4 · 实现后端

复制 [prompts.md](prompts.md) 的「实现后端」Prompt，让 AI 写 `server.js`。

## Step 5 · 实现前端

复制「实现前端」Prompt，让 AI 写聊天界面。

## Step 6 · 安装依赖并运行

```bash
cd ai-chat
npm install
npm start
```

打开浏览器访问 `http://localhost:3000`（端口以 AI 的说明为准）。

## Step 7 · 测试完整流程

输入问题 → 发送 → 看到「思考中…」 → 看到 AI 回答。

## 运行

```bash
npm start
```

## 常见错误

| 现象 | 原因 | 解决 |
| --- | --- | --- |
| 控制台 CORS 报错 | 前端直接调 AI API | 确认请求发到你的后端 `/api/chat` |
| 401 / Invalid key | Key 错误或没读到 | 检查 `.env` 和加载逻辑 |
| 一直「思考中」 | 后端没启动或接口路径不对 | 看后端终端日志和 Network |
| 400 | 模型名或参数格式错 | 对照服务商文档，让 AI 检查 |

更多：[AI API 调用失败](../../debugging/common-errors/ai-api-call-failed.md)

## 下一步

- 加多轮对话记忆（把历史消息一起发给 AI）
- 做 [Tutorial 03 · Todo 应用](../03-first-todo-app/README.md)
- 完整案例见 [Case 003](../../cases/beginner/003-ai-chat/README.md)

## Verification

- 本教程与 [Case 003](../../cases/beginner/003-ai-chat/README.md) 基于同一方案
- Verification: Not Yet Verified（AI API 各家调用方式不同，以官方文档为准）
