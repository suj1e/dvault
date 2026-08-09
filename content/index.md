---
title: dvault
description: 一个用 Markdown 写就的知识保险库
---

# dvault

一个用 Markdown 写就的**知识保险库**。这里有两片区域:

> [!summary] 两个入口
> - 📖 **[[docs/|产品文档]]** —— 产品的使用说明、配置与 API,线性阅读
> - 🌿 **[[garden/|笔记花园]]** —— 知识笔记与想法,网状互链

## 特色

- 🔍 **全文搜索**:右上角搜索框,跨文档和笔记
- 🗺️ **知识图谱**:可视化笔记之间的关联
- 📁 **文件树浏览**:左侧 explorer 按目录组织
- 🌐 **双向链接**:笔记间用 `[[ ]]` 互链,自动生成反向链接
- 🌗 **暗色模式** & **阅读模式**:右上角一键切换
- ✅ 支持 Obsidian 全套语法:任务列表、标注(callout)、LaTeX 公式等

## 如何新增内容

| 放哪 | 怎么做 |
|------|--------|
| 产品文档 | 在 `content/docs/` 下新建 `.md` |
| 知识笔记 | 在 `content/garden/` 下新建 `.md`,尽情用 `[[互链]]` |

写完 `git push origin main`,GitHub Actions 自动构建并部署到 `dvault.flooc.cn`。
