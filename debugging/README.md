# 🐛 Debugging（调试库）

代码报错**并不意味着项目失败**。

报错是软件开发里最正常的事情，连专业程序员每天都会遇到。区别只在于：**会 Debug 的人知道下一步做什么。**

## 核心方法：把问题交给 AI

你只需要三样东西：

1. **错误信息**（完整复制，不要只复制最后一行）
2. **操作过程**（你刚才做了什么）
3. **相关代码**（出错的文件内容，如果知道）

然后交给 AI。参考 [debug-error Prompt](../prompts/debugging/debug-error.md)。

## Debug 五步流程

```text
Error（错误信息）
↓
Reproduce（重现问题：再运行一次，确认能稳定出现）
↓
Find Cause（找到原因：让 AI 分析 + 自己排查）
↓
Fix（修复：一次只改一处）
↓
Test（验证：确认问题消失，且没有引入新问题）
```

## 本库结构

- [common-errors（常见错误）](common-errors/README.md) —— 按错误现象查
- [environment（环境问题）](environment/README.md) —— 安装、版本、端口、密钥
- [frontend（前端问题）](frontend/README.md) —— 页面、样式、交互
- [backend（后端问题）](backend/README.md) —— 接口、数据库、服务器
- [ai（AI 相关问题）](ai/README.md) —— API 调用、模型输出

## Debug Case 模板

每个 Debug Case 包含五个部分：

```text
症状（你看到了什么）
原因（为什么会出现）
排查（怎么一步步确认）
解决（怎么修复）
如何预防（下次怎么避免）
```

新增 Debug Case 时请保持这个结构，并标注 Verification 状态。

## 求助前自检

发 Issue 或问 AI 之前，先确认：

- [ ] 我复制了完整错误信息
- [ ] 我知道自己刚才做了什么操作
- [ ] 我重新运行过一次，确认问题稳定出现
- [ ] 我没有在信息里包含 API Key 或密码

## Verification

- 本库中的案例来自常见开发场景的通用经验
- 每个案例都标注了验证状态
- Verification: Not Yet Verified（案例内容基于通用经验，未在本仓库环境中逐一复现）
