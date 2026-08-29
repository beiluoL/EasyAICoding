# fix-build-error（修复构建错误）

## 适用场景

- 项目安装依赖或构建（Build）时报错
- 出现 `npm install`、`build`、`compile` 之类的失败
- 构建工具报错但你看不懂

## 你需要提供什么

- 完整错误信息：`{{ERROR_MESSAGE}}`
- 你运行的命令：`{{COMMAND}}`
- 环境信息：`{{ENVIRONMENT}}`（Node 版本、Python 版本等，如果知道）

## 完整 Prompt

````text
我的项目构建失败了。

我运行的命令：
{{COMMAND}}

完整错误信息：
```text
{{ERROR_MESSAGE}}
```

我的环境：
{{ENVIRONMENT}}

请这样帮我：
1. 用大白话解释这个构建错误
2. 判断是环境问题（版本不对、缺少依赖）还是代码问题
3. 给出修复步骤，每步附上「预期看到什么」
4. 如果建议安装或升级软件，说明为什么，并提醒我以官方文档为准
5. 不要让我盲目执行删除类命令（如删除 node_modules），如果必须删除，先解释后果
````

## 预期行为

- 明确错误属于环境问题还是代码问题
- 修复步骤可验证
- 对危险命令有解释和提醒

## 常见问题

### 网上说删 node_modules 重装？

可以，但先问 AI：「删除 node_modules 安全吗？删了之后怎么恢复？」不要盲从网上的命令。

## Verification

- 预期行为：见上文
- Verification: Not Yet Verified
