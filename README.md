# Starbucks for Life - 部署指南

## 项目信息

- **项目名称**: Starbucks for Life Guide
- **核心关键词**: Starbucks for Life, Starbucks for Life 2025, free Starbucks
- **目标用户**: 想了解和参与星巴克年度活动的咖啡爱好者

---

## 文件清单

```
starbucks-for-life/
├── index.html     # 主页面（单文件HTML，内联CSS）
├── source.md      # 信息源文档
└── README.md      # 部署指南（本文件）
```

---

## 部署步骤

### Step 1: Git 初始化

```bash
cd E:\热词快站1\starbucks-for-life

# 初始化 Git 仓库
git init

# 添加所有文件
git add .

# 提交
git commit -m "Initial commit: Starbucks for Life landing page"
```

### Step 2: 发布到 GitHub

**方式一：VS Code 操作**
1. 点击左侧"源代码管理"图标
2. 点击"发布到 GitHub"
3. 选择 "Publish to GitHub private repository"
4. 等待发布完成

**方式二：命令行**
```bash
# 在 GitHub 创建新仓库后
git remote add origin https://github.com/你的用户名/starbucks-for-life.git
git branch -M main
git push -u origin main
```

### Step 3: Vercel 部署

1. 访问 [vercel.com](https://vercel.com)
2. 使用 GitHub 账号登录
3. 点击 "Add New" → "Project"
4. 选择 `starbucks-for-life` 仓库
5. 点击 "Import"
6. Framework Preset 选择 "Other"
7. 点击 "Deploy"
8. 等待部署完成（约1分钟）

### Step 4: 绑定自定义域名

**推荐域名**:
- starbucksforlifeguide.com
- starbucks-for-life.guide
- sbuxforlife.com

**Vercel 绑定步骤**:
1. 进入项目 Settings → Domains
2. 输入你的域名，点击 Add
3. 按提示配置 DNS：
   - A 记录: 76.76.21.21
   - 或 CNAME: cname.vercel-dns.com

---

## SEO 提交清单

### Google Search Console
1. 访问 [search.google.com/search-console](https://search.google.com/search-console)
2. 添加资源 → 输入域名
3. DNS 验证（添加 TXT 记录）
4. 提交 sitemap 或首页 URL

### Bing Webmaster
1. 访问 [www.bing.com/webmasters](https://www.bing.com/webmasters)
2. 添加网站
3. 验证所有权
4. 提交 URL

---

## 推广计划

### Day 1 必做
- [ ] 提交 Google Search Console
- [ ] 提交 Bing Webmaster
- [ ] 发布到 1-2 个社交平台

### 推荐平台
- Reddit: r/starbucks, r/freebies
- Twitter/X: 使用 #StarbucksForLife 标签
- Facebook: Starbucks 相关群组

### 外链获取
- 提交到 AI/工具导航站
- 联系咖啡/优惠相关博主

---

## 后续优化

### 内容扩展
- 添加往年获奖者故事
- 添加实时活动倒计时
- 添加用户评论区

### 功能增强
- 添加邮件订阅
- 添加社交分享按钮
- 添加活动提醒功能

---

## 技术说明

- **技术栈**: 纯 HTML + CSS + JavaScript
- **响应式**: 支持移动端和桌面端
- **SEO**: 已优化 Meta 标签、Open Graph、结构化数据
- **性能**: 单文件，无外部依赖（除 Google Fonts）

---

*创建时间: 2025年12月*
