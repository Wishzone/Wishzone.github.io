# Wishzone 个人网站

基于 Jekyll 与 Academic Pages 主题构建的个人项目网站，展示 Hider、WTSIMU、PWTS、YOLO 和 MSSP 等工程与研究实践。

## 内容位置

- 首页：`_pages/about.md`
- 项目列表：`_pages/portfolio.html`
- 项目卡片资料：`_data/projects.yml`
- 项目详情：`_portfolio/*.md`
- 页面样式：`_sass/layout/_portfolio_site.scss`
- 导航：`_data/navigation.yml`

新增项目时，在 `_data/projects.yml` 中加入一条资料，并在 `_portfolio/` 下创建同名 Markdown 文件。详情页的 `project_key`、`permalink` 应与资料中的 `slug` 对应。

## 本地预览

安装 Ruby、Bundler 和 `Gemfile` 中的依赖后运行：

```bash
bundle install
bundle exec jekyll serve
```

然后访问 `http://localhost:4000`。

## 致谢

网站沿用 [Academic Pages](https://github.com/academicpages/academicpages.github.io) / [Minimal Mistakes](https://github.com/mmistakes/minimal-mistakes) 主题的基础结构；其许可信息见仓库中的 `LICENSE`。
