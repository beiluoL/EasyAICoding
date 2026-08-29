# Deployment（部署）

## 定义

**Deployment（部署 / Deploy）**：把软件放到公网上，让别人通过网址访问的过程。

大白话：**部署就是「让软件上线」。** 做完的软件一直放在你自己的电脑上，只有你能用；部署之后，任何有链接的人都能用。

## 例子

你的个人网站在本地运行：

```text
你打开浏览器 → http://localhost:3000 → 只有你的电脑能访问
```

部署之后：

```text
任何人打开 → https://你的网站地址 → 都能访问
```

## 部署需要什么

### 静态网站（最简单）

只有 HTML / CSS / JavaScript 的项目，可以免费部署到：

- GitHub Pages
- Vercel
- Netlify

通常只需要：把代码传到 GitHub → 平台自动构建 → 得到一个公网链接。

### 带后端 / 数据库的项目

需要一台「一直开机的电脑」（服务器）或平台：

- Railway
- Render
- Fly.io
- 云服务器（如阿里云、腾讯云）

还要配置环境变量（比如数据库地址、API Key）。

## 新手最容易踩的坑

### 1. 本地能跑，部署后白屏

常见原因：路径写死（`/style.css` 写成绝对路径）、没有部署静态文件。把现象和错误交给 AI。

### 2. 把 API Key 写进代码

⚠️ 绝对禁止。密钥要放到平台的环境变量（Environment Variable）里，并且永远不要提交到 GitHub。

### 3. 数据库连接不上

部署环境的数据库地址和本地不同，需要重新配置。见 [数据库连接失败](../../debugging/common-errors/database-connection-failed.md)。

## 推荐流程

1. 本地完全跑通
2. 先部署静态版本验证
3. 需要后端再加后端
4. 每次部署都记录链接和问题（用 [development-plan 模板](../../templates/development-plan.md)）

## 相关

- [deploy-project Prompt](../../prompts/deployment/deploy-project.md)
- [Tutorial 03 · Todo 应用（部署部分）](../../tutorials/03-first-todo-app/README.md)

## Verification

- 内容类型：概念解释
- Verification: Not Yet Verified（具体平台的步骤以官方文档为准）
