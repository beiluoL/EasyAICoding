# AGENTS.md — 给 AI 协作者的说明

EasyAICoding 是面向初学者的 AI Coding 开源项目。

## 项目优先级

编辑本仓库内容时，按以下优先级决策：

1. **Beginner Experience（小白体验）** —— 内容默认读者不会编程
2. **Clarity（清晰）** —— 一次只讲一件事，步骤能照着做
3. **Accuracy（准确）** —— 不写没有依据的结论，不写过时命令
4. **Practicality（实用）** —— 能复制、能运行、能验证
5. **Maintainability（可维护）** —— 结构一致、交叉引用、不重复

## 编辑内容时的流程

1. 先阅读 [README.md](README.md)，理解项目定位
2. 再阅读要修改的目录及其 README，理解现有结构
3. 遵循对应 [Template（模板）](templates/README.md)
4. 保持内容与全站一致（术语、风格、链接）
5. 不伪造验证结果：没有实际运行验证，就写 `Not Yet Verified`
6. 不删除已有有效内容：修改优先于删除

## 术语与风格

- 中文为主，技术名词保留英文，例如：Prompt（提示词）、Debug（调试）、Deploy（部署）
- 第一次出现专业术语必须同时给大白话解释
- 避免在 V0.1 内容中使用进阶概念（Agentic Workflow、Context Engineering、State Machine、Reflection、Multi-Agent 等）
- 内容之间互相链接，不复制大量重复内容

## 禁止事项

- 不伪造测试结果、性能数据、兼容性、部署结果、截图、用户数据、Benchmark
- 不提交 API Key、密码、Token
- 不用「这是最好的」「100% 成功」等没有证据的表述
- 不自动 commit、不 push、不创建 GitHub 仓库（除非用户明确要求）
