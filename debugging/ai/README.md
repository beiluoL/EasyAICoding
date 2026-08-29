# AI（AI 相关问题）

AI 相关问题 = 调用 AI 服务、或 AI 生成内容不符合预期。

## 常见类型

| 现象 | 可能原因 | 详细案例 |
| --- | --- | --- |
| 调用报 401 | API Key 错误 | [API Key 错误](../common-errors/api-key-error.md) |
| 调用报 429 | 额度 / 频率限制 | [AI API 调用失败](../common-errors/ai-api-call-failed.md) |
| 调用报 400 | 参数、模型名错误 | [AI API 调用失败](../common-errors/ai-api-call-failed.md) |
| AI 生成内容不对 | Prompt 不清晰、Context 不足 | [ask-ai-correctly Prompt](../../prompts/start/ask-ai-correctly.md) |
| AI「忘记」项目 | 会话上下文丢失 | [Context（上下文）](../../docs/concepts/context.md) |

## AI 问题 Debug 通用步骤

1. **区分问题类型**：是「调用失败」（报错）还是「结果不对」（没报错）？
2. 调用失败 → 看错误码（401 / 429 / 400 / 超时），查 [AI API 调用失败](../common-errors/ai-api-call-failed.md)
3. 结果不对 → 检查 Prompt 是否说清了目标、背景、约束
4. 检查代码里的请求参数（模型名、消息格式）
5. 检查密钥是否放对环境变量

## 核心提醒

**Prompt 是输入，结果不对先改输入。** 不要反复让 AI 重试同一段模糊的 Prompt，先把它写清楚。

## Verification

- 通用方法说明
- Verification: Not Yet Verified
