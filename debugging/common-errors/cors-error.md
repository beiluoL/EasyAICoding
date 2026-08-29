# 跨域（CORS）

## 症状

浏览器控制台报错：

```text
Access to fetch at 'http://localhost:8000/api/todos' from origin
'http://localhost:5173' has been blocked by CORS policy
```

## 原因

浏览器安全机制：网页（`localhost:5173`）请求另一个地址（`localhost:8000`）时，目标服务器没有声明「允许这个来源访问」。

大白话：**浏览器会检查「你从哪来」，服务器没点头，请求就被拦住了。**

## 排查

1. 确认前端地址和后端地址确实不同（端口不同也算跨域）
2. 检查后端有没有配置 CORS（跨域资源共享）
3. 看完整报错，确认是 CORS 拦截而不是其他错误

## 解决

在后端配置 CORS，允许前端地址访问。常见做法：

- Node.js（Express）：安装 `cors` 中间件
- Python（Flask / FastAPI）：使用 `CORS` 配置
- 让 AI 按你的技术栈配置，并只允许你需要的来源，不要 `*` 全开

## 如何预防

- 开发时把前端和后端地址写清楚
- 部署后前后端同域或正确配置 CORS

## Verification

- 基于通用经验
- Verification: Not Yet Verified
