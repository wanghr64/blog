---
title: "Hello, Hugo"
date: 2026-11-23T10:00:00+08:00
tags: ["随笔", "hugo"]
summary: "这个博客的第一次构建：一个没有搜索、没有评论、没有 JavaScript 的站点。"
---

这是一篇示例文章，用来验证排版。删掉它或者改掉它都可以。

## 这个主题有什么

- 首页、文章列表、文章详情、标签页、404
- RSS 与 sitemap（Hugo 自带输出）
- 深色模式（跟随系统，纯 CSS）
- 正文里可以写 Markdown 的常见语法

## 没什么

没有搜索，没有评论，没有统计脚本，没有前端路由。页面就是静态 HTML。

## 一段代码

```go
package main

import "fmt"

func main() {
    fmt.Println("hello, hugo")
}
```

## 一个列表

1. 先写 Markdown
2. 再 `hugo new posts/xxx.md`
3. `git push` 就发布

> 引用也可以，样式保持克制。

行内代码 `hugo server -D` 和 [外链示例](https://gohugo.io/) 都正常。

| 功能 | 状态 |
| --- | --- |
| 标签分类 | 有 |
| 分页 | 有 |
| 站内搜索 | 无 |
