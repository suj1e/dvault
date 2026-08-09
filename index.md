---
title: 首页
nav_order: 1
permalink: /
---

# dvault

一个用 Markdown 写就的知识保险库。

GitHub Pages 会把本仓库根目录下的 Markdown 文件渲染为网页,左侧导航自动收录所有文档,右上角可全文搜索。

## 如何新增文档

1. 在仓库根目录新建 `xxx.md`
2. 顶部填写 front matter:

   ```yaml
   ---
   title: 文档标题       # 显示在导航中
   nav_order: 2          # 决定在侧边栏的排列顺序
   ---
   ```

3. 提交到 `main` 分支,Pages 会自动重新部署
4. 访问 `https://dvault.flooc.cn/xxx.html`

---

Powered by GitHub Pages + Jekyll.
