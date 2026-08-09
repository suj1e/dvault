# dvault

一个用 Markdown 写就的**知识保险库**,基于 [Quartz v5](https://quartz.jzhao.xyz/) 构建,适配 Obsidian 工作流。

🔗 https://dvault.flooc.cn

## 特性

- 🌐 双向链接(`[[互链]]`)+ 反向链接 + 知识图谱
- 🔍 全文搜索 · 📁 文件树浏览 · 🌗 暗色/阅读模式
- 完整支持 Obsidian 语法:callout、任务列表、LaTeX、标签等

## 本地预览

```bash
npm install
npx quartz build --serve
# 打开 http://localhost:8080
```

> 注:`@quartz-community/*` 插件在国内 npm 镜像同步有延迟,本仓库 `.npmrc` 已强制走官方 registry。

## 写作 & 发布

1. 在 `content/` 下新增 `.md` 笔记(可用 Obsidian 编辑)
2. `git push origin main`
3. GitHub Actions 自动构建并部署到 `dvault.flooc.cn`

配置见 `quartz.config.yaml`。
