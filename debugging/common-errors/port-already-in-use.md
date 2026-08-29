# 端口被占用

## 症状

启动项目时报错：

```text
Error: listen EADDRINUSE: address already in use :::3000
```

或：

```text
Port 3000 is already in use
```

## 原因

你要用的端口（例如 3000、5173、8080）已经被另一个程序占用了。

## 排查

1. 看看谁占用了端口（macOS / Linux）：

   ```bash
   lsof -i :3000
   ```

2. 看到输出后，找到 PID（进程 ID）
3. 确认这个进程是不是你自己之前启动、忘记关闭的项目

## 解决

两种方式：

### 方式 1：关闭占用进程（确认是自己启动的项目）

```bash
kill 你的PID
```

> ⚠️ 先确认 PID 对应的程序是什么，不要随便杀系统进程。

### 方式 2：换一个端口

告诉 AI：「把端口从 3000 改成 3001」，或按项目文档修改端口配置。

## 如何预防

- 项目跑完随手停止（Ctrl+C）
- 启动前用 `lsof -i :端口` 检查
- 多个项目使用不同端口

## Verification

- 基于通用经验
- Verification: Not Yet Verified
