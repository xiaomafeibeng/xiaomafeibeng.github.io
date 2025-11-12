# 小马飞奔的博客

基于 [Jekyll](https://jekyllrb.com/) 搭建，并使用 [bit-ranger/blog](https://github.com/bit-ranger/blog) 主题定制。该仓库包含博客的所有源文件，可用于本地预览和部署到 GitHub Pages。

## 本地预览

```powershell
bundle install
bundle exec jekyll serve
```

运行后访问 `http://127.0.0.1:4000` 即可预览站点。

## 主要目录结构

- `_config.yml`：站点配置、分页、评论、搜索等参数。
- `_posts/`：Markdown 博客文章，文件名格式 `YYYY-MM-DD-title.md`。
- `_layouts/`、`_includes/`、`pages/`：主题布局、导航和静态页面。
- `static/`：主题使用的样式、脚本和图片资源。

## 个性化设置

- 若启用 Gitalk 评论，请在 `_config.yml` 的 `comment` 节点填写 `repo`、`client_id`、`client_secret`。
- 若启用 Swiftype 站内搜索，请在 `_config.yml` 的 `swiftype.searchId` 中配置引擎 ID。
- 部署到生产环境时，将 `_config.yml` 中的 `url` 改为你的域名，例如 `https://yourname.github.io/blog`。

## 部署

将仓库推送到 GitHub 并启用 GitHub Pages 即可线上访问：

```powershell
git add .
git commit -m "Update blog"
git push
```

想要自定义更多主题细节，可参考上游主题仓库的文档和示例。

