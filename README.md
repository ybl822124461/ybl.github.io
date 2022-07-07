学术网站的 Github Pages 模板。这是由Stuart Geiger从Minimal Mistakes Jekyll Theme中分叉（然后分离）的，该主题是 © 2016 Michael Rose 并在 MIT 许可下发布。请参阅 LICENSE.md。

我认为我已经让事情顺利进行并修复了一些主要错误，但如果您想改进通用模板/主题，请随时提交问题或提出拉取请求。

# 指示

1. 如果您没有 GitHub 帐户，请注册一个 GitHub 帐户并确认您的电子邮件（必需！）
1. 通过单击右上角的“fork”按钮来分叉此存储库。
1. 转到存储库的设置（以“代码”开头的选项卡中最右边的项目应位于“取消监视”下方）。将存储库重命名为“[您的 GitHub 用户名].github.io”，这也是您网站的 URL。
1. Set site-wide configuration and create content & metadata (see below -- also see [this set of diffs](http://archive.is/3TPas) showing what files were changed to set up [an example site](https://getorg-testacct.github.io) for a user with the username "getorg-testacct")
1. Upload any files (like PDFs, .zip files, etc.) to the files/ directory. They will appear at https://[your GitHub username].github.io/files/example.pdf.  
1. Check status by going to the repository settings, in the "GitHub pages" section
1. (Optional) Use the Jupyter notebooks or python scripts in the `markdown_generator` folder to generate markdown files for publications and talks from a TSV file.

See more info at https://academicpages.github.io/

## To run locally (not on GitHub Pages, to serve on your own computer)
1. Clone the repository and made updates as detailed above
1. Make sure you have ruby-dev, bundler, and nodejs installed: `sudo apt install ruby-dev ruby-bundler nodejs`
1. Run `bundle clean` to clean up the directory (no need to run `--force`)
1. Run `bundle install` to install ruby dependencies. If you get errors, delete Gemfile.lock and try again.
1. Run `bundle exec jekyll serve` to generate the HTML and serve it from localhost:4000


# Changelog -- bugfixes and enhancements

There is one logistical issue with a ready-to-fork template theme like academic pages that makes it a little tricky to get bug fixes and updates to the core theme. If you fork this repository, customize it, then pull again, you'll probably get merge conflicts. If you want to save your various .yml configuration files and markdown files, you can delete the repository and fork it again. Or you can manually patch. 

To support this, here is a manually-curated list of bugs that have been fixed since this project was released. If you have a bug, you can go through and manually update. (If you have a better idea about how to support this, please let me know!)

- 2017-03-27: In author sidebar, link for Google Scholar displays site URL instead of Google Scholar URL in _config.yml
  - [Issue #6](https://github.com/academicpages/academicpages.github.io/issues/6), fixed in [34bg699](https://github.com/academicpages/academicpages.github.io/commit/34bd6990aa335c40cdadc01b5561797860d5eaa6)
- 2017-03-27: Markdown generator is now functioning properly and is well-documented, see the Jupyter notebooks in `markdown_generator`
  - [Issue #8](https://github.com/academicpages/academicpages.github.io/issues/8), fixed in [4528221](https://github.com/academicpages/academicpages.github.io/commit/4528221629bb93508c6ed149b9035d75bb38b402)
