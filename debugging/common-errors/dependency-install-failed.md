# 依赖安装失败

## 症状

安装依赖时报错，例如：

- `npm install` 出现 `ERR!` 或网络错误
- `pip install` 出现 `Could not find a version`
- 安装超时、下载中断

## 原因

常见原因：

1. **网络问题**：下载源访问慢或被墙
2. **版本冲突**：某个依赖要求的版本和已装的冲突
3. **Python 版本不兼容**：`pip` 与项目要求不一致
4. **磁盘或权限问题**：无法写入安装目录

## 排查

1. 复制完整错误信息，找到第一个 `ERR!` 或 `ERROR`
2. 确认网络能访问下载源
3. 确认 Node / Python 版本（`node -v`、`python3 --version`）
4. 国内网络可尝试更换镜像源（npm 淘宝镜像、pip 清华源），但**先问 AI，再执行**

## 解决

以 AI 分析为准。常见做法：

```bash
# npm 重试
npm cache clean --force
npm install

# pip 指定版本
pip install "包名==版本号"
```

⚠️ 不要盲目执行 `rm -rf node_modules`。如果要删除，先问 AI 后果和恢复方式。

## 如何预防

- 记录项目要求的版本（`package.json` / `requirements.txt`）
- 每次换电脑或换目录后，先安装依赖再运行

## Verification

- 基于通用经验
- Verification: Not Yet Verified
