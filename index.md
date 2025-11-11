# YouTube 转录合集

这是一个使用 AI (Gemini 2.5 Flash Lite) 自动转录 YouTube 视频的文稿合集。

## 📺 订阅频道

- Peter Yang
- Dwarkesh Patel
- Lenny's Podcast
- Data-Driven NYC
- Greg Isenberg
- Dialectic
- David Perell
- TKP Podcast
- Every
- Y Combinator

## 🔔 如何订阅

在你的 RSS 阅读器中添加以下链接：

```
https://mungfeing-1210.github.io/youtube-transcripts/feed.xml
```

推荐的 RSS 阅读器：
- Reeder (iOS/macOS)
- NetNewsWire (iOS/macOS)
- Feedly (Web/iOS/Android)
- Inoreader (Web/iOS/Android)

## 📖 最新文稿

{% assign all_pages = site.html_pages | where_exp: "page", "page.path contains '/2025'" | where_exp: "page", "page.name != 'index.md'" | where_exp: "page", "page.title != nil" | sort: 'date' | reverse %}

{% for page in all_pages limit:20 %}
- [{{ page.title }}]({{ page.url }}) - {{ page.channel }}
{% endfor %}

## 🤖 关于

本站所有文稿均由 AI 自动生成，包括：
- 英文字幕转录
- 中文翻译
- 内容摘要 (Key Takeaways)

---

⚡️ Powered by [Gemini 2.5 Flash Lite](https://deepmind.google/technologies/gemini/) & [Jekyll](https://jekyllrb.com/)
