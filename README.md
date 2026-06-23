# 📘 2026 国考备考知识库

基于 **MkDocs Material** 构建的国考备考知识库，支持在线浏览和全文搜索。

## 🌐 在线访问

> 部署后替换为实际地址

- **GitHub Pages**: `https://YOUR_USERNAME.github.io/guokao-kb/`
- **Cloudflare Pages**: `https://guokao-kb.pages.dev`

## 📂 项目结构

```
.
├── mkdocs.yml                    # MkDocs 配置
├── docs/                         # 知识文档（Markdown）
│   ├── index.md                  # 首页
│   ├── overview.md               # 备考规划总览
│   ├── timeline.md               # 备考时间线
│   ├── resources.md              # 学习资源清单
│   ├── changelog.md              # 迭代日志
│   ├── templates/                # 文档模板
│   ├── xingce/                   # 行测模块
│   │   ├── ziliao/               # 资料分析
│   │   ├── panduan/              # 判断推理
│   │   ├── yanyu/                # 言语理解
│   │   ├── shuliang/             # 数量关系
│   │   └── changshi/             # 常识判断
│   ├── shenlun/                  # 申论模块
│   │   ├── guina/                # 归纳概括
│   │   ├── zonghe/               # 综合分析
│   │   ├── tichu/                # 提出对策
│   │   ├── guanche/              # 贯彻执行
│   │   └── dazuowen/             # 大作文
│   ├── zhenti/                   # 真题库
│   └── mokao/                    # 模考记录
├── overrides/                    # 主题覆盖
├── .github/workflows/deploy.yml  # GitHub Actions 部署
└── .gitignore
```

## 🚀 快速开始

### 本地预览

```bash
# 安装依赖
pip install mkdocs-material mkdocs-glightbox

# 本地启动（自动热重载）
mkdocs serve

# 浏览器打开 http://127.0.0.1:8000
```

### 构建静态站点

```bash
mkdocs build
# 输出到 site/ 目录
```

## 📝 如何新增知识文档

1. 复制 `docs/templates/knowledge-template.md`
2. 修改 frontmatter（title、tags、category 等）
3. 填写内容（核心要点、详细内容、B站资源、练习记录）
4. 在 `mkdocs.yml` 的 `nav` 中添加页面链接
5. `git commit` → 自动部署

## 🔄 迭代流程

```
调研/学习 → 落盘为 Markdown → Git commit → GitHub Actions 自动构建 → 网站更新
```

每次迭代在 `docs/changelog.md` 中记录变更。

## 🛠 技术栈

- **构建工具**: [MkDocs Material](https://squidfunk.github.io/mkdocs-material/)
- **部署**: GitHub Pages / Cloudflare Pages
- **CI/CD**: GitHub Actions
- **版本管理**: Git
