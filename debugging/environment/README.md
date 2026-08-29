# Environment（环境问题）

环境问题 = 软件运行的环境（系统、版本、网络、密钥）出了问题。

## 常见类型

| 问题 | 快速判断 | 详细案例 |
| --- | --- | --- |
| 命令找不到 | 终端提示 `command not found` | [项目启动失败](../common-errors/project-start-failed.md) |
| 依赖装不上 | 安装时报 `ERR!` / `ERROR` | [依赖安装失败](../common-errors/dependency-install-failed.md) |
| 端口冲突 | `EADDRINUSE` | [端口被占用](../common-errors/port-already-in-use.md) |
| 数据库连不上 | `ECONNREFUSED` | [数据库连接失败](../common-errors/database-connection-failed.md) |
| 密钥错误 | `Invalid API key` / `401` | [API Key 错误](../common-errors/api-key-error.md) |

## 环境问题 Debug 通用步骤

1. **先确认版本**：`node -v`、`python3 --version`、`npm -v`
2. **确认目录**：`pwd`（你不在预期目录，命令自然找不到）
3. **确认服务**：数据库、后端服务是否在运行
4. **确认网络**：下载源、外部 API 是否可达
5. **确认密钥**：环境变量是否已设置、值是否正确

## 环境信息模板

问 AI 或提交 Issue 时，附上：

```text
操作系统：macOS 14 / Windows 11 / Ubuntu 22.04
工具版本：Node v20.x、Python 3.11、npm 10.x
项目位置：/Users/xxx/my-website
我运行的命令：npm run dev
完整错误信息：……
```

## Verification

- 通用方法说明
- Verification: Not Yet Verified
