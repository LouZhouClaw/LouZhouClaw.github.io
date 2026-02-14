# Ziheng Wu

个人主页 / Personal GitHub Pages site.

## 本地预览

用浏览器直接打开 `index.html`，或本地起一个静态服务：

```bash
# Python 3
python3 -m http.server 8000

# 或 npx
npx serve .
```

然后访问 http://localhost:8000

## 发布到 GitHub Pages

1. 在 GitHub 新建仓库，仓库名建议：`你的用户名.github.io`（例如 `wuziheng.github.io`），这样发布后地址为 `https://wuziheng.github.io`。
2. 将本目录内容推送到该仓库：
   ```bash
   cd /Users/wzh/Desktop/cursor/githubio
   git init
   git add index.html README.md .nojekyll
   git commit -m "Initial commit: personal site"
   git branch -M main
   git remote add origin https://github.com/你的用户名/你的用户名.github.io.git
   git push -u origin main
   ```
3. 在仓库 **Settings → Pages** 中：
   - **Source** 选 **Deploy from a branch**
   - **Branch** 选 `main`，目录选 **/ (root)**
   - 保存后等待 1–2 分钟，访问 `https://你的用户名.github.io` 即可。

若仓库名不是 `用户名.github.io`，则地址为 `https://你的用户名.github.io/仓库名/`。

## 内容说明

- 单页静态站点，无构建步骤，直接由 GitHub Pages 托管。
- 内容整理自个人简历与项目介绍，tech 风格、适合技术向展示。
