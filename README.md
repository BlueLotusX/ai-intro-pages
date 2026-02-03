# AI 介绍网页

本仓库包含两个静态网页，可通过 GitHub Pages 公网访问。

## 启用 GitHub Pages 后访问地址

假设你的 GitHub 用户名为 `你的用户名`，仓库名为 `WebPages`（或你实际创建的仓库名），则：

- **首页（本目录）**：`https://你的用户名.github.io/仓库名/`
- **AI 介绍页**：`https://你的用户名.github.io/仓库名/ai_intro.html`
- **AI 介绍页（含隐藏内容）**：`https://你的用户名.github.io/仓库名/ai_intro_hidden.html`

## 如何部署到 GitHub 并开启公网访问

1. 在 GitHub 上新建一个仓库（例如命名为 `ai-intro-pages`），不要勾选「Initialize with README」。
2. 在本地本目录（WebPages）下执行：
   ```bash
   git init
   git add .
   git commit -m "Add AI intro pages"
   git branch -M main
   git remote add origin https://github.com/你的用户名/仓库名.git
   git push -u origin main
   ```
3. 在 GitHub 仓库页面：**Settings → Pages**，在 **Source** 中选择 **Deploy from a branch**，Branch 选 **main**，Folder 选 **/ (root)**，保存。
4. 等待一两分钟，即可通过 `https://你的用户名.github.io/仓库名/` 访问上述网页。

## 文件说明

- `index.html`：首页，提供到两个子页面的链接
- `ai_intro.html`：介绍「什么是 AI」的页面
- `ai_intro_hidden.html`：内容相同，HTML 中含不显示但可被爬虫抓取的注释文字
