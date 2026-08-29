# Tutorial 04 · 第一个 RAG 应用

## 你要做什么

做一个「基于你的文档回答问题」的应用：上传或放入几篇文章，然后问 AI 关于这些文章的问题。

这就是 RAG（Retrieval-Augmented Generation，检索增强生成）的入门实现。

> 大白话：**先把资料切成小块存起来，提问时先找到相关的块，再让 AI 基于这些块回答。** 这样 AI 能回答「只属于你资料」的问题。

## 最终会得到什么

一个本地应用：加载文档 → 提问 → 得到基于文档的回答。

## 准备工作

- 完成 [Tutorial 02](../02-first-ai-chat/README.md)（会调用 AI API）
- 完成 [Tutorial 03](../03-first-todo-app/README.md)（会做基本应用）
- Node.js 环境
- 一份你自己的资料（几篇 Markdown 或文本文件即可）
- 约 3-4 小时

## Step 1 · 理解 RAG 的三个环节

```text
1. 加载：把文档读进来
2. 切分 + 存储：切成小块，存进「向量数据库」（Vector Database）
3. 问答：提问 → 找到相关块 → 连同问题发给 AI
```

先不用懂「向量」是什么，把这三个环节记住就行，让 AI 实现。

## Step 2 · 创建项目

新建文件夹 `rag-app`，复制 [prompts.md](prompts.md) 的「创建结构」Prompt。

## Step 3 · 实现加载和切分

用「实现加载切分」Prompt，让 AI 实现文档读取和切分。

## Step 4 · 实现问答

用「实现问答」Prompt，让 AI 实现：提问 → 检索 → 生成回答。

## Step 5 · 实现简单界面

一个页面：显示资料加载状态 + 提问框 + 回答区。

## Step 6 · 运行验证

```bash
npm install
npm start
```

放入你的资料，问几个只有资料能回答的问题：

- 「资料里提到的最重要建议是什么？」
- 「根据资料，步骤二是怎么做的？」

如果 AI 答不上来或答错，看 [常见错误](#常见错误)。

## 运行

```bash
npm start
```

## 常见错误

| 现象 | 原因 | 解决 |
| --- | --- | --- |
| 回答与资料无关 | 没检索到相关内容 | 检查文档是否加载成功、切分是否太粗 |
| 上下文太长报错 | 把整个文档发给 AI 了 | 确认实现的是「先检索再发送」 |
| 401 / 额度错误 | Key 或额度问题 | 查 [AI API 调用失败](../../debugging/common-errors/ai-api-call-failed.md) |
| 向量库报错 | 依赖安装或版本问题 | 让 AI 检查依赖和版本，以官方文档为准 |

## 下一步

- 支持更多文件格式（PDF、Word）
- 做 [Tutorial 05 · AI 工具](../05-first-ai-tool/README.md)（毕业项目）
- 深入理解可看 [Database（数据库）](../../docs/concepts/database.md) 和 [Deployment（部署）](../../docs/concepts/deployment.md)

## Verification

- RAG 实现方式各家不同（向量库、嵌入模型），本教程只给方向
- Verification: Not Yet Verified（具体实现以 AI 生成的方案和官方文档为准）
