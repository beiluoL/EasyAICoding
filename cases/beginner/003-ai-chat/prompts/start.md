# Case 003 · 开始 Prompt

## 第一步：创建结构

```text
我完全不会编程，想做一个人工智能聊天网页。请先帮我创建项目骨架，先不要写功能代码：

技术栈：Node.js + Express（后端）+ 原生 HTML/CSS/JavaScript（前端）

项目结构：
ai-chat/
├── server.js          # 后端，负责调用 AI API
├── public/
│   ├── index.html
│   ├── style.css
│   └── script.js
├── .env               # 环境变量（不提交）
├── .gitignore
└── package.json

要求：
- .gitignore 里必须包含 .env
- 先告诉我每个文件是干什么的，我确认后再创建
```

## 第二步：实现后端转发

```text
请在 server.js 里实现：
1. 读取 .env 里的 API_KEY
2. 提供 POST /api/chat 接口：接收 { message }，调用 AI API 返回回答
3. AI API 的调用方式请使用 {{你的服务商}} 的官方 SDK 或标准接口
4. 调用失败时返回可读的错误信息，不要泄露 Key
5. 用中文注释解释每一部分
```

## 第三步：实现前端

```text
请在 public/ 里实现聊天界面：
1. 输入框 + 发送按钮 + 对话显示区
2. 发送后显示「思考中…」，拿到回答后显示
3. 出错时在页面上显示错误提示
4. 请求失败时按钮恢复可用
5. 界面简洁，代码有中文注释
```
