# YouTube Transcripts - AI 自动转录合集

这是一个使用 AI (Gemini 2.5 Flash Lite) 自动转录 YouTube 视频的文稿合集，支持 RSS 订阅。

## 🚀 快速开始

### 1. 创建 GitHub 仓库

在 GitHub 上创建一个新仓库，例如 `youtube-transcripts`

### 2. 初始化 Git 并推送

```bash
cd youtube-reader/output

# 初始化 Git
git init

# 添加所有文件
git add .

# 创建初始提交
git commit -m "Initial commit: Setup Jekyll RSS feed"

# 设置 main 分支
git branch -M main

# 添加 GitHub 远程仓库（替换成你的仓库地址）
git remote add origin git@github.com:你的用户名/youtube-transcripts.git

# 推送到 GitHub
git push -u origin main
```

### 3. 启用 GitHub Pages

1. 进入 GitHub 仓库 Settings
2. 找到 Pages 设置
3. Source 选择 `main` 分支
4. 点击 Save

等待 1-2 分钟，你的网站就会部署到：
```
https://你的用户名.github.io/youtube-transcripts/
```

### 4. 订阅 RSS

在你的 RSS 阅读器中添加：
```
https://你的用户名.github.io/youtube-transcripts/feed.xml
```

### 5. 更新配置

编辑 `_config.yml`，将以下内容替换为你的信息：
- `url`: 替换 `USERNAME` 为你的 GitHub 用户名
- `baseurl`: 替换 `REPO_NAME` 为你的仓库名

## 🤖 自动化

每次运行 `youtube_reader_agent.py` 后，如果有新的转录文稿，会自动：
1. 创建 Git commit
2. 推送到 GitHub
3. GitHub Pages 自动部署
4. RSS feed 自动更新

## 📱 推荐的 RSS 阅读器

- **iOS/macOS**: Reeder, NetNewsWire
- **Android**: Feedly, Inoreader
- **Web**: Feedly, The Old Reader

## 📁 目录结构

```
output/
├── _config.yml              # Jekyll 配置
├── feed.xml                 # RSS feed 模板
├── index.md                 # 首页
├── .gitignore              # Git 忽略文件
├── processed_videos.json   # 已处理视频记录
├── Peter-Yang/
│   └── 2025-11-11/
│       └── *.md            # 转录文稿
├── Dwarkesh-Patel/
│   └── 2025-11-11/
│       └── *.md
└── ...
```

## 🎯 功能特性

- ✅ AI 自动转录（英文 → 中文）
- ✅ 生成内容摘要 (Key Takeaways)
- ✅ RSS feed 订阅
- ✅ 按频道分类组织
- ✅ 去重机制（避免重复处理）
- ✅ 自动推送到 GitHub
- ✅ GitHub Pages 托管

## 🔧 技术栈

- [Gemini 2.5 Flash Lite](https://deepmind.google/technologies/gemini/) - AI 模型
- [yt-dlp](https://github.com/yt-dlp/yt-dlp) - YouTube 下载工具
- [Jekyll](https://jekyllrb.com/) - 静态网站生成器
- [GitHub Pages](https://pages.github.com/) - 免费托管

## 📝 许可

MIT License
