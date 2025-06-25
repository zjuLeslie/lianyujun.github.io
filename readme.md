
## 如何生成个人主页

我的个人主页是基于 [Chi Zhang](https://chizapoth.github.io/) ([github](https://github.com/chizapoth/chizapoth.github.io)) 的个人主页修改而来的。 

制作过程如下：

1. 克隆 [lianyujun.github.io](https://github.com/lianyujun/lianyujun.github.io)。
   - 在 GitHub 上创建一个新的仓库，命名为 `{你的账号}.github.io`，例如 `lianyujun.github.io`。
   - 使用 GitHub Desktop 或者命令行工具将仓库克隆到本地。
2. 修改、更新你的个人信息：
   - 修改 `index.qmd` 文件，添加个人信息、头像、社交链接等。
   - 将 **images** 文件夹中的头像图片替换为你自己的。
   - 修改 `_quarto.yml` 文件，更新网站标题、作者信息等。
   - 修改 `publications.qmd`, `blog.qmd` 等文件，添加你的学术论文、项目、博客等。
3. 在 VScode 中编译上述文件，生成网页文件：
   - 在 VScode 中打开 `index.qmd` 文件
   - 按快捷键 `Ctrl + ~`，打开终端，确认当前目录为 `{你的账号}.github.io`，否则，可以使用 `cd {你的账号}.github.io` 命令切换目录。
   - 输入并执行 `quarto render` 命令，编译生成网页文件。
   - 网页文件会生成在 `docs` 文件夹中，打开此文件夹，双击 `index.html` 文件查看效果。
   - 将 `docs` 文件夹中的所有文件复制到仓库根目录下。注意：需要复制的是 `docs` 文件夹中的所有文件，而 `docs` 文件夹。
4. 将修改后的代码推送到 GitHub：
   - 在 GitHub Desktop 中，点击 `Commit to main` 按钮，提交修改。
   - 点击 `Push origin` 按钮，将修改推送到 GitHub。
5. 配置 github pages：
   - 在 GitHub 仓库页面，点击 `Settings`。
   - 在 `Pages` 部分，选择 `main` 分支作为源，并设置 `/ (root)` 目录。
   - 点击 `Save` 按钮。
   - 等待几分钟，GitHub 会自动生成并部署你的个人主页。
   - 访问 `https://{你的账号}.github.io` 查看效果。这就是你的个人主页地址了。

## 配置要求

我是在 VScode 中使用 [Quarto](https://quarto.org/) 编译的，以下是一些配置要求：

- **Quarto**：安装 [Quarto](https://quarto.org/docs/get-started/) 工具。
- **VScode**：安装 [Visual Studio Code](https://code.visualstudio.com/) 编辑器。
  - 安装 [Quarto 插件](https://marketplace.visualstudio.com/items?itemName=quarto.quarto)。
  - 安装 [Markdown 插件](https://marketplace.visualstudio.com/items?itemName=DavidAnson.vscode-markdownlint)。
- **github desktop** (可选，但强烈建议)：安装 [GitHub Desktop](https://desktop.github.com/) 客户端，用于管理代码仓库。