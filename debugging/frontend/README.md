# Frontend（前端问题）

前端问题 = 用户看到的界面出了问题。

## 常见类型

| 现象 | 可能原因 | 详细案例 |
| --- | --- | --- |
| 页面空白 | HTML / JS 报错、文件 404 | [前端页面空白](../common-errors/blank-page.md) |
| 样式不对 | CSS 路径错误、选择器写错 | 问 AI + [debug-error Prompt](../../prompts/debugging/debug-error.md) |
| 按钮没反应 | JavaScript 报错 | [前端页面空白](../common-errors/blank-page.md) |
| 接口请求失败 | 404 / 500 / CORS | [接口 404](../common-errors/api-404.md)、[接口 500](../common-errors/api-500.md)、[跨域](../common-errors/cors-error.md) |

## 前端 Debug 通用步骤

1. 按 **F12** 打开浏览器开发者工具
2. 看 **Console（控制台）**：复制所有红色错误
3. 看 **Network（网络）**：找 404 / 500 的请求
4. 看 **Elements（元素）**：确认页面结构是否按预期渲染
5. 把错误信息 + 现象发给 AI

## 前端报错怎么看

控制台错误通常长这样：

```text
Uncaught TypeError: Cannot read properties of null (reading 'addEventListener')
```

大白话：**代码想给一个不存在的元素绑定点击事件。** 通常是元素没加载或 ID 写错了。

## Verification

- 通用方法说明
- Verification: Not Yet Verified
