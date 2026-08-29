# Case 003 · Verification（验证）

## 如何运行

```bash
cd ai-chat
npm install
npm start
```

然后打开浏览器访问 `http://localhost:3000`（端口以实际为准）。

## 如何验证

| 检查项 | 操作 | 预期结果 |
| --- | --- | --- |
| 页面打开 | 访问 localhost | 显示聊天界面 |
| 发送问题 | 输入文字 → 发送 | 显示「思考中…」 |
| AI 回答 | 等待几秒 | 显示 AI 的回答 |
| 错误处理 | 先清空 .env 再发送 | 页面显示可读错误，不白屏 |
| 密钥安全 | 搜索代码 | 前端代码和仓库里没有真实 Key |
| 控制台 | F12 | 无红色错误 |

## 预期结果

- 完成一轮完整对话
- 加载状态可见
- 错误有提示
- `.env` 未被提交（`git status` 看不到它）

## Verification

- 待实际操作后填写
- Not Yet Verified
