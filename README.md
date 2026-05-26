# 孙琦的简历主页

这是孙琦的个人简历网站仓库,包含多个版本的简历和项目展示。

## 📁 项目结构

```
github-pages-homepage/
├── index.html              # 主页面
├── styles.css              # 样式文件
├── .nojekyll              # 禁用 Jekyll 处理
├── .github/
│   └── workflows/
│       └── deploy.yml      # GitHub Pages 自动部署配置
├── assets/
│   ├── profile.png         # 头像照片
│   ├── resume.pdf          # Hackathon 简历 PDF
│   └── images/             # 其他图片资源
│       ├── 证件照.png
│       ├── lang-resume.png
│       └── lang-resume-2.png
└── docs/                   # 各类简历文档
    ├── 孙琦-复试简历.docx
    ├── 孙琦-简历基础信息.md
    ├── 孙琦-AI产品经理简历.html
    ├── 孙琦-AI产品经理简历.md
    ├── hackathon-resume.html
    └── project.md
```

## 🚀 特性

- **响应式设计**: 适配桌面和移动设备
- **多版本简历**: 包含面向不同场景的简历版本
  - AI 产品经理简历
  - Hackathon 竞赛简历
  - 研究生复试简历
- **自动部署**: 通过 GitHub Actions 自动部署到 GitHub Pages
- **项目展示**: 详细的项目经验和技能展示

## 🌐 在线访问

访问 GitHub Pages 部署的网站后,可以在线查看简历和下载 PDF 版本。

## 💻 本地开发

1. 克隆仓库:
   ```bash
   git clone <your-repo-url>
   cd github-pages-homepage
   ```

2. 本地预览:
   - 直接用浏览器打开 `index.html` 文件
   - 或使用本地服务器:
     ```bash
     # Python 3
     python -m http.server 8000
     
     # Node.js
     npx http-server
     ```

3. 访问 `http://localhost:8000`

## 📝 更新简历

1. 编辑 `index.html` 文件更新网页内容
2. 更新 `docs/` 目录下的各类简历文档
3. 提交更改:
   ```bash
   git add .
   git commit -m "Update resume"
   git push
   ```

4. GitHub Actions 会自动部署更新

## 🛠️ 部署方式

1. 新建一个 GitHub 仓库,例如 `sunqi-homepage`
2. 将本目录下的所有文件推送到仓库的 `main` 分支
3. 进入 GitHub 仓库的 `Settings` → `Pages`
4. Source 选择 `GitHub Actions`
5. 推送后等待 Actions 执行完成,即可获得 GitHub Pages 访问地址

如果你使用 `用户名.github.io` 作为仓库名,也可以直接作为个人主页根站点访问。

## 📧 联系方式

详见简历中的联系信息。

## 📄 许可

此项目仅用于个人简历展示。
