# 项目启动失败

## 症状

运行项目时，终端直接报错退出，或页面打开失败。常见错误包括：

- `command not found`
- `Cannot find module`
- `Error: listen EADDRINUSE`
- 启动后立即闪退

## 原因

最常见的原因：

1. **命令不对**：你运行的命令和项目要求的不一致
2. **依赖没装**：项目需要的依赖库没有安装
3. **入口文件缺失或改名**：项目找不到启动文件
4. **版本不兼容**：Node / Python 等版本和项目要求不一致

## 排查

按顺序检查：

1. 确认你在**项目根目录**里运行命令（用 `pwd` 查看当前目录）
2. 对照项目的 README，确认启动命令正确
3. 确认依赖已安装（Node 项目看 `node_modules` 是否存在，Python 项目看 `venv` 是否存在）
4. 检查入口文件是否存在（例如 `index.html`、`app.py`、`package.json` 里的 `main`）

把完整错误信息发给 AI，使用 [debug-error Prompt](../../prompts/debugging/debug-error.md)。

## 解决

常见修复：

```bash
# 安装依赖（Node 项目）
npm install

# Python 项目
pip install -r requirements.txt

# 确认在正确目录
cd 你的项目目录
```

具体以 AI 的分析和项目 README 为准。

## 如何预防

- 每个项目根目录放一个 README，写清启动命令
- 安装依赖后不要随便移动项目文件夹
- 报错时完整复制错误信息，不要只看最后一行

## Verification

- 基于通用经验
- Verification: Not Yet Verified
