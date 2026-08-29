# Case 002 · Steps（步骤）

## Step 1 · 创建项目

新建文件夹 `todo-app`，用 AI 工具打开它。

## Step 2 · 让 AI 生成基础版本

复制 [start.md](prompts/start.md)，发给 AI。

## Step 3 · 运行验证基础功能

打开页面，测试：添加、完成、删除。

**完成标志**：MVP 五项功能都能用。

## Step 4 · 让 AI 加统计功能

用 [modify-code Prompt](../../../prompts/coding/modify-code.md) 让 AI 加「已完成数量」和「清空已完成」。

## Step 5 · 每次修改都验证

每改一个功能：刷新 → 测试 → 看控制台。有报错就用 [debug.md](prompts/debug.md)。

## Step 6 · 故意弄坏再修好

练习 Debug：让 AI 故意改错一行代码，观察报错，再用 Debug Prompt 修复。这是最好的学习方式。

## Step 7 · 记录

完成 [verification.md](verification.md)，读 [lessons.md](lessons.md)。

## 完成标准

- [ ] MVP 五项功能可用
- [ ] 统计功能可用
- [ ] 控制台无报错
- [ ] 我完成了一次 Debug 练习
