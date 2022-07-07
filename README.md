学术网站的 Github Pages 模板。这是由Stuart Geiger从Minimal Mistakes Jekyll Theme中分叉（然后分离）的，该主题是 © 2016 Michael Rose 并在 MIT 许可下发布。请参阅 LICENSE.md。

我认为我已经让事情顺利进行并修复了一些主要错误，但如果您想改进通用模板/主题，请随时提交问题或提出拉取请求。

注意：如果您正在使用此存储库并且现在收到有关安全漏洞的通知，请删除 Gemfile.lock 文件。
指示
如果您没有 GitHub 帐户，请注册一个 GitHub 帐户并确认您的电子邮件（必需！）
通过单击右上角的“fork”按钮来分叉此存储库。
转到存储库的设置（以“代码”开头的选项卡中最右边的项目应位于“取消监视”下方）。将存储库重命名为“[您的 GitHub 用户名].github.io”，这也是您网站的 URL。
设置站点范围的配置并创建内容和元数据（见下文——另见这组差异显示哪些文件已更改，以便为用户名“getorg-testacct”的用户设置示例站点）
将任何文件（如 PDF、.zip 文件等）上传到 files/ 目录。它们将出现在 https://[你的 GitHub 用户名].github.io/files/example.pdf。
通过转到“GitHub 页面”部分中的存储库设置来检查状态
（可选）使用文件夹中的 Jupyter 笔记本或 python 脚本markdown_generator从 TSV 文件生成用于出版物和演讲的降价文件。
在https://academicpages.github.io/上查看更多信息

在本地运行（不在 GitHub Pages 上，在您自己的计算机上提供服务）
克隆存储库并进行更新，如上所述
确保您安装了 ruby​​-dev、bundler 和 nodejs：sudo apt install ruby-dev ruby-bundler nodejs
运行bundle clean清理目录（无需运行--force）
运行bundle install以安装 ruby​​ 依赖项。如果出现错误，请删除 Gemfile.lock 并重试。
运行bundle exec jekyll liveserve以生成 HTML 并从localhost:4000本地服务器提供它将在更改时自动重建和刷新页面。
变更日志——错误修正和增强
像学术页面这样的现成模板主题存在一个后勤问题，这使得修复错误和更新核心主题变得有点棘手。如果你 fork 这个存储库，对其进行自定义，然后再次拉取，你可能会遇到合并冲突。如果你想保存你的各种 .yml 配置文件和 markdown 文件，你可以删除存储库并再次 fork 。或者你可以手动打补丁。

为了支持这一点，对底层代码的所有更改都显示为带有“代码更改”标签的已关闭问题——在此处获取列表。每个问题线程都包含链接到单个提交的注释或多个提交之间的差异，因此具有分叉存储库的人可以轻松识别他们需要修补的内容。
