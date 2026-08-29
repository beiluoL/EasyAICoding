# 贡献指南

感谢你想参与 EasyAICoding！这是一个面向初学者的 AI Coding 开源项目，我们欢迎所有人贡献。

## 欢迎贡献什么

- **Tutorial（教程）** —— 一步步教小白做出真实项目的教程
- **Prompt（提示词）** —— 有完整说明、能直接复制使用的 Prompt
- **Case（案例）** —— 真实做出来的项目记录
- **Debug Case（调试案例）** —— 真实遇到并解决过的错误
- **Documentation（文档）** —— 修正错别字、补充说明、改进表达

## 贡献的基本要求

### 1. 内容清晰

- 面向零基础用户，第一次出现的专业术语必须同时给大白话解释
- 一次只讲一件事，步骤要能照着做

### 2. 可复现

- 每一步都要写出「做什么」和「预期看到什么」
- 提供 Expected Result（预期结果）
- 没有实际跑过，就写 `Not Yet Verified`，不要写「亲测有效」

### 3. 不能伪造

禁止伪造测试结果、性能数据、截图、用户数据。

### 4. 不能泄露密钥

- 永远不要提交 API Key、密码、Token
- 示例中的密钥一律使用占位符，例如 `sk-你的KEY`
- 如果发现自己不小心提交了密钥，请立即联系维护者并轮换该密钥

## 提交流程

### 第一次贡献

1. Fork 这个仓库（GitHub 页面右上角的 Fork 按钮）
2. Clone 到本地：

   ```bash
   git clone https://github.com/你的用户名/EasyAICoding.git
   ```

3. 创建自己的分支：

   ```bash
   git checkout -b docs/add-my-tutorial
   ```

4. 修改或添加内容
5. 提交并推送
6. 到 GitHub 上创建 Pull Request

### Pull Request 要求

- 标题清楚说明改动内容，例如 `docs: add first-ai-tool tutorial`
- 描述里说明：改了什么、为什么改、如何验证
- 保持改动范围小，一个 PR 解决一个问题

## 内容模板

新增内容请先使用仓库中的模板，保持全站风格一致：

- [Tutorial 模板](templates/tutorial.md)
- [Prompt 模板](templates/prompt.md)
- [Bug Report 模板](templates/bug-report.md)
- [Case 模板](cases/README.md)
- [Debug Case 模板](debugging/README.md)

## 风格约定

- 中文为主，技术名词保留英文，例如：Prompt（提示词）、Debug（调试）
- 不要用「这是最好的」「100% 成功」这类没有证据的表述
- 内容之间要互相链接，不要复制粘贴重复内容

## 审核流程

维护者会检查：

1. 内容是否符合 [内容质量标准](docs/contribution/content-quality.md)
2. 是否可复现、不伪造
3. 链接和 Markdown 格式是否正确
4. 是否泄露敏感信息

审核可能需要几天时间，请耐心等待。我们欢迎讨论，但请保持友善。

## 更多

- [行为准则](CODE_OF_CONDUCT.md)
- [支持](SUPPORT.md)
