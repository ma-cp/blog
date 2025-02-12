---
title: "记github-pages"
date: 2025-02-12
category: programmer
tags: git
published: true
---

# 记录我的blog的诞生以及git的使用

这个blog是以“GitHub Pages”为基础的，选择它是因为这足够简单，而且有清晰的教学。

最初的一步是从[github-pages](https://github.com/skills/github-pages)这个仓库开始的，中间会有GitHub的bot帮忙引导。

整个blog是支持md语法的。

文件名中的日期是github-pages用来识别并创建页面的，所以不能乱写，而只能写真实的。

## 使用GitHub

GitHub是用于“版本控制”的。版本控制更像是对团队而言的一个功能。

版本控制，对个人来说很少有人会将自己的作品分成多个“版本”，一个人用GitHub更像是为自己的行为留下“操作记录”。

版本控制，对团队合作来说是多人“创建各自的版本”，git起到一个写完代码之后“合并版本”的作用。

一个仓库以其main为核心可以有很多个分支，最主流的就是至少会分一个develop分支用于开发，在develop分支中将内容commit，最后将develop中的内容合并到main分支，完成一个开发循环。

GitHub有成熟的网页支持，可以直接在GitHub网页中更改内容，此时只需commit，内容便直接传到了云端。

而如果要在本地用ide写代码，需要将仓库克隆下来，此时修改本地文件并进行commit之后，文件只是由本地的软件git确认了，需要进一步地push来将本地更改同步到云端。

在本地使用clone只会将“某一个”分支克隆下来，即，commit和push只会改变这一个分支的内容，要合并分支应该去GitHub的网页中操作。（网页中会展示更多的信息，有利于清晰的判断合并的正确性。）

SourceTree是一个成熟的GUI工具用于管理git，其优于GitHubDesktop的地方在于有清晰的“树状图谱”，能够令人更清晰地观察一个仓库中的分支信息。

GitHub的网页端和SourceTree的组合可以完全避免使用命令行来控制版本管理。

## md语法

既然用github-pages就免不了使用一些md语法。

首先，Markdown 是 HTML 的父集，所以任何 HTML 文件都是有效的 Markdown。

md中空一行来表示换行。

代码的语法是：`这些内容会被原封不动地显示出来`。

注释的语法是：`<!--`开头，`-->`结尾。

标题的语法是：`#`，一个井号代表一级标题，两个井号代表二级小标题，井号越多标题越小，一般一级标题要保留给整篇文章的title，从两个井号开始做小标题。

链接的语法是：`[显示文字](https://链接的地址.com)`，在md语法下直接一个地址会引起格式错误，所以应采用这个复杂一点的写法。

其它和md有影响的符号：`+-*`、`>`表示引用、`1.`表示列表。

更多详细的语法可以参见：[learnXinYmin](https://learnxinyminutes.com/zh-cn/markdown/)



