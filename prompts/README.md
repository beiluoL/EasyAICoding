# 💬 Prompt Library（提示词库）

这里的 Prompt 都可以直接复制使用。每个 Prompt 都包含：适用场景、你需要提供什么、完整 Prompt、预期行为、常见问题。

## 使用方式

1. 找到适合你场景的 Prompt
2. 复制全文
3. 把 `{{占位符}}` 替换成你的内容
4. 发给 AI

## 目录

### 开始（Start）

- [start-project（开始项目）](start/start-project.md) ⭐ 最重要，从想法开始
- [explain-project（解释项目）](start/explain-project.md)
- [ask-ai-correctly（正确提问）](start/ask-ai-correctly.md)

### 编码（Coding）

- [implement-feature（实现功能）](coding/implement-feature.md)
- [explain-code（解释代码）](coding/explain-code.md)
- [modify-code（修改代码）](coding/modify-code.md)

### 调试（Debugging）

- [debug-error（排查报错）](debugging/debug-error.md)
- [analyze-stacktrace（分析错误堆栈）](debugging/analyze-stacktrace.md)
- [fix-build-error（修复构建错误）](debugging/fix-build-error.md)

### 测试（Testing）

- [write-tests（编写测试）](testing/write-tests.md)
- [verify-feature（验证功能）](testing/verify-feature.md)

### 部署（Deployment）

- [deploy-project（部署项目）](deployment/deploy-project.md)

## 使用原则

1. **一个 Prompt 解决一个问题**
2. **替换占位符再发送**，不要直接发 `{{}}`
3. **AI 跑偏就纠正**：直接回复「先不要写代码」「按我第 2 点做」
4. **效果取决于工具和模型**：如果某个工具不响应 Prompt 中的某个要求，用自然语言补充说明

## 贡献 Prompt

想提交新 Prompt？请使用 [Prompt 提交模板](../.github/ISSUE_TEMPLATE/prompt-submission.yml) 并遵循 [内容质量标准](../docs/contribution/content-quality.md)。

## Verification

- 每个 Prompt 都标注了预期行为
- 实际效果因工具、模型、上下文而异
- Verification: Not Yet Verified（未在全部工具上逐一验证）
