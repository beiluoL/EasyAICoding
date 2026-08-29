# Level 4 — 我可以 Debug / Test / Deploy

## 目标

- 遇到错误不慌，按流程解决
- 学会基本测试和验证
- 把自己的项目部署上线

## 需要知道什么

- Debug 流程：Error → Reproduce → Find Cause → Fix → Test（[调试库](../../debugging/README.md)）
- 常见错误分类：环境、前端、后端、AI（[分类目录](../../debugging/README.md)）
- 什么是部署（Deploy，把项目放到公网让别人能用）

## 推荐 Prompt

- [debug-error](../../prompts/debugging/debug-error.md)
- [analyze-stacktrace](../../prompts/debugging/analyze-stacktrace.md)
- [fix-build-error](../../prompts/debugging/fix-build-error.md)
- [write-tests](../../prompts/testing/write-tests.md)
- [verify-feature](../../prompts/testing/verify-feature.md)
- [deploy-project](../../prompts/deployment/deploy-project.md)

## 推荐 Tutorial

- [Tutorial 03 · 第一个 Todo 应用](../../tutorials/03-first-todo-app/README.md)（后半部分：部署）
- [Tutorial 05 · 第一个 AI 工具](../../tutorials/05-first-ai-tool/README.md)

## 练习项目

1. 故意制造一个错误（比如把文件名改错），用 [Debug 流程](../../debugging/README.md) 解决它
2. 给你的 Todo 项目写 3 条测试（用 [write-tests](../../prompts/testing/write-tests.md)）
3. 用免费平台部署你的个人网站，得到一个公网链接

## 毕业标准

- [ ] 我能独立解决 2 个不同类型的错误
- [ ] 我的项目有自动化测试或明确的验证步骤
- [ ] 我的项目部署上线，有公开链接

## 下一步

→ [Level 5 — 我可以独立使用 AI 构建软件](level-5.md)
