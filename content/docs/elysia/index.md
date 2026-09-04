---
title: Elysia
description: Harness 产品
---

# Elysia

类似 DeepSeek Harness 的 Coding Agent 产品，可以真正操作代码库、执行命令、验证结果，并支持 Web、macOS、iOS 三端访问和控制。

## 文档结构

### 产品
- [[产品/产品定位|产品定位]] —— 是什么、给谁用、价值主张、与 Harness 的差异
- [[产品/产品模型|产品模型]] —— Device、Workspace、Session、Task、Agent、Tool Execution、Events
- [[产品/V1范围|V1 范围]] —— V1 完整闭环与明确不包含的功能
- [[产品/非目标|非目标]] —— V1 明确不做的事情
- [[产品/用户流程|用户流程]] —— 8 个核心用户故事 + Agent Loop
- [[产品/核心原则|核心原则]] —— 7 条产品设计原则

### 设计
- [[设计/信息架构|信息架构]] —— 三端导航结构与页面层级

### 开发
- [[开发/数据模型|数据模型]] —— 核心数据结构与存储方案
- [[开发/事件系统|事件系统]] —— Event System 设计与 Event 列表
- [[开发/权限矩阵|权限矩阵]] —— V1 权限设计（无账户体系）
- [[开发/异常与边界|异常与边界]] —— 异常场景与边界处理

### 测试
- [[测试/验收标准|验收标准]] —— V1 验收标准与完成定义

### 参考
- [[术语表|术语表]] —— 专有名词解释
- [[待确认问题|待确认问题]] —— 产品与工程待决策问题

---

> [!important] V1 核心闭环
> User → Client → Session → Agent → Tools → Workspace → Execution → Verification → Events → Clients
>
> **Agent First、Execution Is Real、Native Clients、One Session Multiple Clients、Device Is First-class、Protocol Before UI、V1 Must Be Small**

---

> [!note] 如何新增文档
> 在 `elysia/` 下新建 `.md` 文件，顶部写 `title`，正文用 Markdown。支持子目录分级。
