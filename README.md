# 博客

Hugo + GitHub Pages。零 JavaScript、无搜索、无第三方依赖的极简主题。

## 本地预览

```sh
hugo server -D
```

打开 <http://localhost:1313>。

## 写文章

```sh
hugo new posts/我的文章.md
```

文件里的 `draft: true` 改成 `false`（或者本地预览时加 `-D`）。

## 目录结构

```
hugo.toml                 站点配置（标题、导航、每页篇数）
content/
  _index.md               首页简介
  posts/                  文章
  tags/_index.md          标签页
  about.md                关于页
layouts/
  baseof.html             公共骨架
  home.html               首页
  list.html               分区列表（/posts/）
  term.html               单个标签页
  taxonomy.html           标签总览（/tags/）
  single.html             文章页
  404.html
  _partials/              head / header / crumbs / footer / post-list
assets/
  css/main.css            主题样式（含深色模式）
  css/chroma.css          代码高亮配色
  favicon.svg
.github/workflows/hugo.yml  推送到 main 即部署
```

## 部署

推到 `main` 分支后，GitHub Actions 自动构建并发布到 Pages。
仓库 Settings → Pages → Source 需要选 **GitHub Actions**。

`baseURL` 由 workflow 里的 `actions/configure-pages` 自动注入，仓库改名或换自定义域名都不用改 `hugo.toml`。

## 改样式

颜色和间距都在 `assets/css/main.css` 顶部的 `:root` 变量里。
