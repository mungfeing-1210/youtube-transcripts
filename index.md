---
layout: home
title: YouTube 转录合集
---

<style>
/* Substack 风格优化 */
body {
  font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, "Helvetica Neue", Arial, sans-serif;
  line-height: 1.6;
  color: #1a1a1a;
}

.hero {
  text-align: center;
  padding: 3rem 0 2rem;
  max-width: 680px;
  margin: 0 auto;
}

.hero h1 {
  font-family: Georgia, "Times New Roman", serif;
  font-size: 2.2rem;
  font-weight: 600;
  margin-bottom: 0.8rem;
  letter-spacing: -0.02em;
}

.hero-subtitle {
  font-size: 1.1rem;
  color: #757575;
  margin-bottom: 1.2rem;
}

.rss-link {
  display: inline-block;
  padding: 0.6rem 1.4rem;
  background: transparent;
  color: #667eea;
  text-decoration: none;
  border: 1.5px solid #667eea;
  border-radius: 20px;
  font-size: 0.95rem;
  font-weight: 500;
  transition: all 0.2s ease;
}

.rss-link:hover {
  background: #667eea;
  color: white;
  transform: translateY(-1px);
}

/* 频道筛选区 */
.channel-filters {
  margin: 2rem 0;
  padding: 1.2rem;
  background: #fafafa;
  border-radius: 12px;
}

.filters-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(140px, 1fr));
  gap: 0.7rem;
}

.channel-filter {
  padding: 0.65rem 1rem;
  background: white;
  color: #4a4a4a;
  border: 1px solid #e0e0e0;
  border-radius: 20px;
  cursor: pointer;
  font-size: 0.9rem;
  font-weight: 500;
  transition: all 0.2s ease;
}

.channel-filter:hover {
  border-color: #667eea;
  color: #667eea;
  transform: translateY(-2px);
  box-shadow: 0 2px 8px rgba(102, 126, 234, 0.15);
}

.channel-filter.active {
  background: #667eea;
  color: white;
  border-color: #667eea;
}

/* 文章列表 */
#articles-list {
  margin: 3rem 0;
  max-width: 720px;
  margin-left: auto;
  margin-right: auto;
}

.article-card {
  padding: 1.8rem 0;
  margin-bottom: 0;
  border-bottom: 1px solid #f0f0f0;
  background: transparent;
  transition: all 0.2s ease;
}

.article-card:hover {
  background: #fafafa;
  padding-left: 1rem;
  padding-right: 1rem;
  margin-left: -1rem;
  margin-right: -1rem;
  border-radius: 8px;
  border-bottom-color: transparent;
}

.article-title {
  margin: 0 0 0.6rem 0;
  font-family: Georgia, "Times New Roman", serif;
  font-size: 1.45rem;
  font-weight: 600;
  line-height: 1.4;
  letter-spacing: -0.01em;
}

.article-title a {
  text-decoration: none;
  color: #1a1a1a;
  transition: color 0.2s ease;
}

.article-title a:hover {
  color: #667eea;
}

.article-meta {
  display: flex;
  align-items: center;
  gap: 0.8rem;
  font-size: 0.9rem;
  color: #757575;
}

.article-channel {
  font-weight: 500;
}

.article-date {
  color: #999;
}

.article-divider {
  color: #ddd;
}

/* 页脚 */
.site-footer {
  text-align: center;
  padding: 3rem 0 2rem;
  margin-top: 4rem;
  border-top: 1px solid #f0f0f0;
  color: #999;
  font-size: 0.9rem;
}

.site-footer a {
  color: #757575;
  text-decoration: none;
  transition: color 0.2s ease;
}

.site-footer a:hover {
  color: #667eea;
}

.footer-divider {
  margin: 0 0.8rem;
  color: #ddd;
}
</style>

<!-- Hero 区域 -->
<div class="hero">
  <h1>YouTube 转录合集</h1>
  <p class="hero-subtitle">每日更新 10+ 优质频道的 AI 转录文稿</p>
  <a href="{{ site.baseurl }}/feed.xml" class="rss-link">🔔 订阅 RSS</a>
</div>

<!-- 订阅频道筛选 -->
<div class="channel-filters">
  <div class="filters-grid">
    <button class="channel-filter active" data-channel="all">全部</button>
    <button class="channel-filter" data-channel="Peter Yang">Peter Yang</button>
    <button class="channel-filter" data-channel="Dwarkesh Patel">Dwarkesh Patel</button>
    <button class="channel-filter" data-channel="Lenny's Podcast">Lenny's Podcast</button>
    <button class="channel-filter" data-channel="The MAD Podcast with Matt Turck">Data-Driven NYC</button>
    <button class="channel-filter" data-channel="Greg Isenberg">Greg Isenberg</button>
    <button class="channel-filter" data-channel="Dialectic Podcast with Jackson Dahl">Dialectic</button>
    <button class="channel-filter" data-channel="David Perell">David Perell</button>
    <button class="channel-filter" data-channel="The Knowledge Project Podcast">TKP Podcast</button>
    <button class="channel-filter" data-channel="Every">Every</button>
    <button class="channel-filter" data-channel="Y Combinator">Y Combinator</button>
  </div>
</div>

<!-- 转录文章列表 -->
<div id="articles-list">
{% assign all_pages = site.html_pages | where_exp: "page", "page.title != nil" | where_exp: "page", "page.channel != nil" | sort: 'date' | reverse %}

{% for page in all_pages limit:20 %}
<article class="article-card" data-channel="{{ page.channel }}">
  <h2 class="article-title">
    <a href="{{ site.baseurl }}{{ page.url }}">{{ page.title }}</a>
  </h2>
  <div class="article-meta">
    <span class="article-channel">{{ page.channel }}</span>
    <span class="article-divider">·</span>
    <time class="article-date">{{ page.date | date: "%Y 年 %m 月 %d 日" }}</time>
  </div>
</article>
{% endfor %}
</div>

<script>
document.addEventListener('DOMContentLoaded', function() {
  const filterButtons = document.querySelectorAll('.channel-filter');
  const articles = document.querySelectorAll('.article-card');

  filterButtons.forEach(button => {
    button.addEventListener('click', function() {
      const selectedChannel = this.getAttribute('data-channel');

      // 更新按钮样式
      filterButtons.forEach(btn => {
        if (btn === this) {
          btn.classList.add('active');
        } else {
          btn.classList.remove('active');
        }
      });

      // 筛选文章
      articles.forEach(article => {
        const articleChannel = article.getAttribute('data-channel');
        if (selectedChannel === 'all' || articleChannel === selectedChannel) {
          article.style.display = 'block';
        } else {
          article.style.display = 'none';
        }
      });
    });
  });
});
</script>

<!-- 页脚 -->
<div class="site-footer">
  <p>
    <a href="#about">关于本站</a>
    <span class="footer-divider">|</span>
    <a href="{{ site.baseurl }}/feed.xml">RSS订阅</a>
    <span class="footer-divider">|</span>
    <span>Powered by <a href="https://deepmind.google/technologies/gemini/" target="_blank">Gemini 2.5</a> & <a href="https://jekyllrb.com/" target="_blank">Jekyll</a></span>
  </p>
</div>
