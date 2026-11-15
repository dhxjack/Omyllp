# 自由 · On Liberty

一个关于「自由」的个人博客：法律的边界、哲学的追问，与 Linux 的开源精神。

线上地址：<https://blog.lianglianglaw.cn/>

## 文件结构

```
.
├── index.html              首页：首屏 + 三个板块卡片（卡片内列出该板块文章）
├── assets/
│   └── style.css           全站共用样式，改配色只需动这一个文件
├── articles/
│   ├── _template.html      文章模板，复制后改名使用
│   └── one-html-blog.html  已发布文章
└── README.md
```

## 发一篇新文章

1. 复制 `articles/_template.html`，重命名为英文小写短横线形式，例如 `kejixianzhi.html`；
2. 替换文件里所有 `【】` 占位内容（标题、摘要、日期、目录、正文）；
3. 打开 `index.html`，在对应板块的 `<ul class="post-list">` 里加一条：

```html
<li>
  <time datetime="2026-11-20">11.20</time>
  <a href="articles/kejixianzhi.html">文章标题</a>
</li>
```

4. 把 `index.html` 和 `articles/` 下的新文件一起上传到 GitHub，帽子云自动构建。

## 本地预览

纯静态站点，直接双击 `index.html` 即可查看，无需安装环境。注意样式在外部 CSS 文件里，需保持 `assets/` 目录结构完整。

## 部署

推送到 `main` 分支后由帽子云自动构建发布。

- 构建命令：留空
- 输出目录：仓库根目录（留空）
- CDN 缓存 20 分钟，更新后强刷 `Ctrl/Cmd + Shift + R`

## 内容

法律 / LINUX / 哲学 三个板块，持续完善中。
