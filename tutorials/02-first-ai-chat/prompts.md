# Tutorial 02 · Prompts

## 创建结构

```text
我完全不会编程，想做一个 AI 聊天网页。先创建项目骨架，先不要写功能代码：

技术栈：Node.js + Express + 原生 HTML/CSS/JavaScript

项目结构：
ai-chat/
├── server.js
├── public/
│   ├── index.html
│   ├── style.css
│   └── script.js
├── .env
├── .gitignore
└── package.json

要求：
- .gitignore 必须包含 .env
- 先告诉我每个文件的作用，我确认后再创建
```

## 实现后端

```text
请在 server.js 里实现 POST /api/chat 接口：
1. 从 .env 读取 API_KEY
2. 接收 { message }，调用 {{你的AI服务商}} 的 API 返回回答
3. 调用方式以官方 SDK 为准
4. 失败时返回可读错误，不泄露 Key
5. 中文注释解释每部分
```

## 实现前端

```text
请在 public/ 里实现聊天界面：
1. 输入框 + 发送按钮 + 对话区
2. 发送后显示「思考中…」，拿到回答后显示
3. 出错时页面显示可读错误
4. 界面简洁，中文注释
```

## Debug

```text
AI 聊天项目报错。
现象：{{描述}}
完整错误信息：{{粘贴}}
我的服务商：{{服务商}}
请用大白话解释原因，给最小修复方案。
```
