# Case 004 · Steps（步骤）

## Step 1 · 准备数据库

让 AI 配置 SQLite，创建 `posts` 表（标题、内容、创建时间）。

## Step 2 · 实现文章 CRUD

实现接口：

- `GET /api/posts` 文章列表
- `POST /api/posts` 新建文章
- `GET /api/posts/:id` 文章详情
- `DELETE /api/posts/:id` 删除文章

## Step 3 · 实现前端页面

列表页 + 新建页 + 详情页。

## Step 4 · 验证 MVP

按 [verification.md](verification.md) 验证 CRUD。**重启项目，确认数据还在。**

## Step 5 · 接入 AI 生成草稿

在新建页加一个功能：输入主题 → 调用 AI 生成文章草稿 → 填入编辑框。复用 Case 003 的后端转发方式。

## Step 6 · 编辑功能（可选）

加 `PUT /api/posts/:id` 更新接口和编辑页面。

## Step 7 · 记录

完成验证表，读 [lessons.md](lessons.md)。

## 完成标准

- [ ] MVP CRUD 全部可用
- [ ] 数据重启后还在
- [ ] AI 生成草稿可用
- [ ] 代码结构清晰
