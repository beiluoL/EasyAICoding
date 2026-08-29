# Case 004 · Verification（验证）

## 如何运行

```bash
cd ai-blog
npm install
npm start
```

访问 `http://localhost:3000`。

## 如何验证

| 检查项 | 操作 | 预期结果 |
| --- | --- | --- |
| 新建文章 | 新建页填写 → 保存 | 跳回列表，新文章出现 |
| 持久化 | 重启项目（Ctrl+C 再 start） | 文章还在 |
| 详情 | 点击文章 | 显示标题和内容 |
| 删除 | 点删除 | 文章从列表消失 |
| AI 草稿 | 输入主题 → 生成 | 草稿填入编辑框 |
| 错误提示 | 清空 .env 再生成 | 显示可读错误 |
| 密钥安全 | 搜索仓库 | 无真实 Key |

## 预期结果

- CRUD 完整可用
- 重启后数据不丢
- AI 草稿能生成

## Verification

- 待实际操作后填写
- Not Yet Verified
