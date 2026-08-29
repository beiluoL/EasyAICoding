# Tutorial 05 · 第一个 AI 工具

## 你要做什么

做你自己的 AI 工具：一个解决真实问题的小产品。这是毕业项目，把前四个教程的能力组合起来。

## 最终会得到什么

一个属于你的、能用的 AI 工具，有需求文档、验证记录和部署计划。

## 准备工作

- 完成 Tutorial 01-04（或同等能力）
- 一个真实想法
- 每周 3-5 小时，持续 1-2 周

## Step 1 · 确定想法

用 [project-idea 模板](../../templates/project-idea.md) 写下想法。

好的 V0.1 工具标准：

- 解决一个你真实遇到的问题
- 核心功能只有一个
- 不需要登录、支付等复杂功能

例子（仅供参考）：

- 文章摘要器：粘贴链接或文字，输出摘要
- 英文写作助手：帮你改语法、润色
- 周报生成器：输入本周工作，生成周报
- 菜谱助手：输入冰箱里的食材，给出菜谱

## Step 2 · 写需求

用 [requirement 模板](../../templates/requirement.md) 写：功能清单、MVP、验收标准。

## Step 3 · 拆任务

用 [start-project Prompt](../../prompts/start/start-project.md) 让 AI 把项目拆成小任务。

## Step 4 · 搭建骨架

复用已学的技术栈（Node.js + Express + 原生前端，需要保存数据就加 SQLite）。

## Step 5 · 一个一个实现

每个任务走完整循环：

```text
实现 → 运行 → 验证 → 记录 → 下一个
```

用 [development-plan 模板](../../templates/development-plan.md) 跟踪进度。

## Step 6 · 打磨体验

让 AI 改进：错误提示、加载状态、界面整洁度、空状态。

## Step 7 · 部署计划

用 [deploy-project Prompt](../../prompts/deployment/deploy-project.md) 了解部署方案。V0.1 至少完成「部署计划」，能实际部署更好。

## Step 8 · 记录成 Case

按 [Case 标准](../../cases/README.md) 记录你的项目，提交到 EasyAICoding（[贡献指南](../../CONTRIBUTING.md)），或者放进你的作品集。

## 运行

```bash
npm install
npm start
```

## 常见错误

| 现象 | 原因 | 解决 |
| --- | --- | --- |
| 功能越加越多 | 忘了 MVP | 回到需求文档，砍掉 P1/P2 |
| AI 改乱了旧功能 | 一次改太多 | 一次一个任务，用 [modify-code Prompt](../../prompts/coding/modify-code.md) |
| 不知道下一步 | 任务太大 | 让 AI 再拆小，直到「一眼知道怎么做」 |
| 做一半想放弃 | 目标太大 | 把「能跑起来」当第一步目标，先有 MVP 再谈完美 |

## 下一步

- 部署上线，把链接分享给朋友
- 完成 [Learning Roadmap Level 5](../../docs/roadmap/level-5.md) 的毕业标准
- 为 EasyAICoding 贡献你的项目记录

## Verification

- 本教程是流程指南，不包含具体项目代码
- Verification: Not Yet Verified（每个项目需要独立验证）
