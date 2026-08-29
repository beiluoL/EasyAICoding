# API Key 错误

## 症状

调用 AI 或第三方服务时报错：

- `Invalid API key`
- `401 Unauthorized`
- `Authentication failed`
- `Missing API key`

## 原因

常见原因：

1. **Key 写错了**：复制漏字符、多了空格
2. **Key 放错地方**：代码里找不到、环境变量名不匹配
3. **Key 已失效**：过期、被撤销、额度用完
4. **Key 不属于当前服务**：用了别的平台的 Key

## 排查

1. 确认 Key 完整且没有多余空格
2. 确认 Key 放的位置正确（环境变量 or 配置文件），且**没有提交到 GitHub**
3. 到服务商控制台确认 Key 状态（有效 / 过期）
4. 检查请求里是否真的带上了 Key（让 AI 帮你看日志）

## 解决

- 重新生成一个 Key，更新到环境变量
- 重启项目让新的环境变量生效
- 如果 Key 泄露过（比如误提交过），**立即撤销并重新生成**

## 如何预防

- Key 只放环境变量，`.env` 文件加入 `.gitignore`
- 永远不要截图或复制 Key 到聊天里发给别人
- 用 `grep` 检查代码里有没有硬编码的 Key（见 [validate-content workflow](../../.github/workflows/validate-content.yml)）

## Verification

- 基于通用经验
- Verification: Not Yet Verified
