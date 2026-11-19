# blog-home

[www.qzmer.me](https://www.qzmer.me) 的主页 —— Better call Jamie!

一个纯静态页面（`index.html`），没有构建步骤，部署在 Vercel。链到「他说」[say.qzmer.me](https://say.qzmer.me)（主）和「玩意」[blog.qzmer.me](https://blog.qzmer.me)（存档）。

## 本地预览

```bash
python3 -m http.server 3200
# 打开 http://localhost:3200
```

## 旧链接跳转

博客原来在 `www.qzmer.me` 下，搬到 `blog.qzmer.me` 后，`vercel.json` 把首页以外的所有路径 301 到博客的同名路径（查询参数原样保留），旧的文章链接和 RSS 订阅地址都不会失效。

主页以后加新页面时，需要在跳转规则里把它排除掉（站点图标 `favicon.ico`、`icon.svg`、`apple-touch-icon.png` 已排除）。
