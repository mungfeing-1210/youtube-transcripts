---
layout: default
title: YouTube 转录合集
---

<div style="text-align: center; padding: 2rem 0;">
  <h1 style="font-size: 2.5rem; margin-bottom: 1rem;">📚 YouTube 转录合集</h1>
  <p style="font-size: 1.2rem; color: #666; max-width: 600px; margin: 0 auto;">
    使用 AI 自动转录优质 YouTube 视频，提供中英双语文稿和内容摘要
  </p>
</div>

---

## 🔔 订阅 RSS

<div style="background: linear-gradient(135deg, #667eea 0%, #764ba2 100%); padding: 2rem; border-radius: 12px; color: white; margin: 2rem 0;">
  <h3 style="margin-top: 0; color: white;">一键订阅，第一时间获取新内容</h3>
  <div style="background: rgba(255,255,255,0.2); padding: 1rem; border-radius: 8px; margin: 1rem 0;">
    <code style="color: white; font-size: 0.95rem; word-break: break-all;">https://mungfeing-1210.github.io/youtube-transcripts/feed.xml</code>
  </div>
  <p style="margin-bottom: 0; font-size: 0.9rem; opacity: 0.9;">
    复制上方链接，添加到你喜欢的 RSS 阅读器中
  </p>
</div>

### 推荐的 RSS 阅读器

<div style="display: grid; grid-template-columns: repeat(auto-fit, minmax(200px, 1fr)); gap: 1rem; margin: 1.5rem 0;">
  <div style="padding: 1rem; border: 1px solid #e1e8ed; border-radius: 8px;">
    <strong>🍎 iOS/macOS</strong><br/>
    Reeder, NetNewsWire
  </div>
  <div style="padding: 1rem; border: 1px solid #e1e8ed; border-radius: 8px;">
    <strong>🌐 Web/跨平台</strong><br/>
    Feedly, Inoreader
  </div>
</div>

---

## 📖 最新文稿

<div style="margin: 2rem 0;">
{% assign all_pages = site.html_pages | where_exp: "page", "page.title != nil" | where_exp: "page", "page.channel != nil" | sort: 'date' | reverse %}

{% for page in all_pages limit:20 %}
<div style="padding: 1.5rem; margin-bottom: 1rem; border: 1px solid #e1e8ed; border-radius: 8px; transition: box-shadow 0.3s;">
  <h3 style="margin-top: 0; margin-bottom: 0.5rem;">
    <a href="{{ page.url }}" style="text-decoration: none; color: #1a1a1a;">{{ page.title }}</a>
  </h3>
  <div style="display: flex; gap: 1rem; font-size: 0.9rem; color: #666;">
    <span>📺 {{ page.channel }}</span>
    <span>📅 {{ page.date | date: "%Y-%m-%d" }}</span>
  </div>
</div>
{% endfor %}
</div>

---

## 📺 订阅频道

<div style="display: grid; grid-template-columns: repeat(auto-fit, minmax(150px, 1fr)); gap: 0.8rem; margin: 1.5rem 0;">
  <div style="padding: 0.8rem; background: #f7fafc; border-radius: 6px; text-align: center;">Peter Yang</div>
  <div style="padding: 0.8rem; background: #f7fafc; border-radius: 6px; text-align: center;">Dwarkesh Patel</div>
  <div style="padding: 0.8rem; background: #f7fafc; border-radius: 6px; text-align: center;">Lenny's Podcast</div>
  <div style="padding: 0.8rem; background: #f7fafc; border-radius: 6px; text-align: center;">Data-Driven NYC</div>
  <div style="padding: 0.8rem; background: #f7fafc; border-radius: 6px; text-align: center;">Greg Isenberg</div>
  <div style="padding: 0.8rem; background: #f7fafc; border-radius: 6px; text-align: center;">Dialectic</div>
  <div style="padding: 0.8rem; background: #f7fafc; border-radius: 6px; text-align: center;">David Perell</div>
  <div style="padding: 0.8rem; background: #f7fafc; border-radius: 6px; text-align: center;">TKP Podcast</div>
  <div style="padding: 0.8rem; background: #f7fafc; border-radius: 6px; text-align: center;">Every</div>
  <div style="padding: 0.8rem; background: #f7fafc; border-radius: 6px; text-align: center;">Y Combinator</div>
</div>

---

## 🤖 关于本站

<div style="background: #f7fafc; padding: 2rem; border-radius: 12px; margin: 2rem 0;">
  <h3 style="margin-top: 0;">AI 自动生成的内容</h3>
  <p>本站所有文稿均由 AI 自动转录和翻译，每篇文章包含：</p>
  <ul style="margin-bottom: 0;">
    <li><strong>英文字幕转录</strong> - 完整的英文原文</li>
    <li><strong>中文翻译</strong> - 流畅准确的中文翻译</li>
    <li><strong>Key Takeaways</strong> - 核心观点提取和结构化摘要</li>
  </ul>
</div>

<div style="text-align: center; padding: 2rem 0; color: #666; font-size: 0.9rem;">
  <p>⚡️ Powered by <a href="https://deepmind.google/technologies/gemini/" target="_blank">Gemini 2.5 Flash Lite</a> & <a href="https://jekyllrb.com/" target="_blank">Jekyll</a></p>
</div>
