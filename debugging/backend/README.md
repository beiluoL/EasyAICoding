# Backend（后端问题）

后端问题 = 数据、逻辑、接口出了问题。

## 常见类型

| 现象 | 可能原因 | 详细案例 |
| --- | --- | --- |
| 接口 404 | 路径 / 方法不匹配、服务没启动 | [接口 404](../common-errors/api-404.md) |
| 接口 500 | 后端代码异常、数据库错误 | [接口 500](../common-errors/api-500.md) |
| 数据保存不了 | 数据库连接失败 | [数据库连接失败](../common-errors/database-connection-failed.md) |
| 浏览器拦截请求 | CORS 未配置 | [跨域](../common-errors/cors-error.md) |

## 后端 Debug 通用步骤

1. **看后端日志**：终端输出或日志文件，找异常堆栈
2. **复现请求**：用浏览器直接访问接口地址，看返回
3. **检查请求**：路径、方法、参数、Headers
4. **检查依赖**：数据库、外部服务是否正常
5. 用 [analyze-stacktrace Prompt](../../prompts/debugging/analyze-stacktrace.md) 分析堆栈

## 后端报错怎么看

后端日志里最常见的：

```text
Error: connect ECONNREFUSED 127.0.0.1:5432
```

大白话：**代码想连接本机 5432 端口（通常是数据库），但那里没有服务在听。**

## Verification

- 通用方法说明
- Verification: Not Yet Verified
