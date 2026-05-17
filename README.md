# 孙琦个人主页

这是一个适合部署到 GitHub Pages 的静态个人主页，包含个人介绍、项目经历、技能栈、联系方式以及 PDF 简历下载。

## 目录结构

- `index.html`：主页内容
- `styles.css`：页面样式
- `assets/profile.png`：个人照片
- `assets/resume.pdf`：PDF 简历
- `.nojekyll`：关闭 GitHub Pages 的 Jekyll 处理
- `.github/workflows/deploy.yml`：GitHub Pages 自动部署工作流

## 部署方式

1. 新建一个 GitHub 仓库，例如 `sunqi-homepage`。
2. 将本目录下的所有文件推送到仓库的 `main` 分支。
3. 进入 GitHub 仓库的 `Settings` → `Pages`。
4. Source 选择 `GitHub Actions`。
5. 推送后等待 Actions 执行完成，即可获得 GitHub Pages 访问地址。

如果你使用 `用户名.github.io` 作为仓库名，也可以直接作为个人主页根站点访问。
