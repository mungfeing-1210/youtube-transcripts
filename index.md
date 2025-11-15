---
layout: home
title: YouTube 转录合集
---

<style>
/* Every 风格优化 - 现代编辑设计 */
body {
  font-family: "Inter", -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, "Helvetica Neue", Arial, sans-serif;
  font-size: 18px;
  line-height: 1.7;
  color: #1a1a1a;
  background: #ffffff;
}

/* Hero 区域 - 紧凑高效 */
.hero {
  text-align: center;
  padding: 1.5rem 2rem 1rem;
  max-width: 760px;
  margin: 0 auto;
  margin-bottom: 1.5rem;
}

.hero h1 {
  font-family: "Tiempos Text", Georgia, "Times New Roman", serif;
  font-size: 2rem;
  font-weight: 700;
  margin-bottom: 0.6rem;
  letter-spacing: -0.03em;
  line-height: 1.1;
  color: #0a0a0a;
}

.hero-subtitle {
  font-size: 1rem;
  color: #6b6b6b;
  margin-bottom: 1.2rem;
  line-height: 1.5;
  font-weight: 400;
}

.rss-link {
  display: inline-block;
  padding: 1rem 2.2rem;
  background: #0a0a0a;
  color: white;
  text-decoration: none;
  border-radius: 30px;
  font-size: 1rem;
  font-weight: 600;
  transition: all 0.3s cubic-bezier(0.4, 0, 0.2, 1);
  box-shadow: 0 4px 14px rgba(0, 0, 0, 0.1);
}

.rss-link:hover {
  background: #2a2a2a;
  transform: translateY(-2px);
  box-shadow: 0 6px 20px rgba(0, 0, 0, 0.15);
}

/* 频道筛选区 - 更宽更紧凑 */
.channel-filters-wrapper {
  margin: 1.5rem auto;
  max-width: 1100px;
  padding: 0 2rem;
}

.channel-filters-title {
  margin: 0 0 1rem 0;
  font-family: "Tiempos Text", Georgia, "Times New Roman", serif;
  font-size: 1.3rem;
  font-weight: 700;
  color: #0a0a0a;
  text-align: left;
  letter-spacing: -0.02em;
}

.channel-filters {
  padding: 1.2rem 2rem;
  background: #f8f9fa;
  border-radius: 16px;
  box-shadow: 0 1px 3px rgba(0, 0, 0, 0.04);
}

.filters-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(140px, 1fr));
  gap: 0.8rem;
}

.channel-filter {
  padding: 0.7rem 1.2rem;
  background: white;
  color: #2a2a2a;
  border: 2px solid #e5e7eb;
  border-radius: 30px;
  cursor: pointer;
  font-size: 0.9rem;
  font-weight: 600;
  transition: all 0.25s cubic-bezier(0.4, 0, 0.2, 1);
  text-align: center;
  box-shadow: 0 1px 2px rgba(0, 0, 0, 0.04);
}

.channel-filter:hover {
  border-color: #0a0a0a;
  color: #0a0a0a;
  transform: translateY(-3px);
  box-shadow: 0 4px 12px rgba(0, 0, 0, 0.08);
}

.channel-filter.active {
  background: #0a0a0a;
  color: white;
  border-color: #0a0a0a;
  box-shadow: 0 4px 12px rgba(0, 0, 0, 0.15);
}

/* 文章列表 - 紧凑高效 */
#articles-list {
  margin: 2rem auto;
  max-width: 1000px;
  padding: 0 2rem;
}

.articles-section-title {
  margin: 0 0 1.5rem 0;
  font-family: "Tiempos Text", Georgia, "Times New Roman", serif;
  font-size: 1.3rem;
  font-weight: 700;
  color: #0a0a0a;
  text-align: left;
  letter-spacing: -0.02em;
}

.article-card {
  padding: 1.5rem 1.5rem;
  margin-bottom: 0;
  border-bottom: 2px solid #f0f0f0;
  background: transparent;
  transition: all 0.3s cubic-bezier(0.4, 0, 0.2, 1);
}

.article-card:hover {
  background: #fafbfc;
  padding-left: 2rem;
  padding-right: 2rem;
  margin-left: -2rem;
  margin-right: -2rem;
  border-radius: 12px;
  border-bottom-color: transparent;
  box-shadow: 0 2px 8px rgba(0, 0, 0, 0.04);
}

.article-title {
  margin: 0 0 0.8rem 0;
  font-family: "Inter", -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, "Helvetica Neue", Arial, sans-serif;
  font-size: 1.3rem;
  font-weight: 700;
  line-height: 1.35;
  letter-spacing: -0.02em;
}

.article-title a {
  text-decoration: none;
  color: #0a0a0a;
  transition: color 0.2s ease;
}

.article-title a:hover {
  color: #4a4a4a;
}

.article-meta {
  display: flex;
  align-items: center;
  gap: 1rem;
  font-size: 1rem;
  color: #6b6b6b;
}

.article-channel {
  font-weight: 600;
  color: #2a2a2a;
}

.article-date {
  color: #9b9b9b;
  font-weight: 400;
}

.article-divider {
  color: #d0d0d0;
}

/* 页脚 - 更简洁 */
.site-footer {
  text-align: center;
  padding: 4rem 2rem 3rem;
  margin-top: 6rem;
  border-top: 2px solid #f0f0f0;
  color: #9b9b9b;
  font-size: 0.95rem;
}

.site-footer a {
  color: #6b6b6b;
  text-decoration: none;
  transition: color 0.2s ease;
  font-weight: 500;
}

.site-footer a:hover {
  color: #0a0a0a;
}

.footer-divider {
  margin: 0 1rem;
  color: #d0d0d0;
}

/* Toast 提示 */
.toast {
  position: fixed;
  top: 6rem;
  left: 50%;
  transform: translateX(-50%);
  background: #f0f0f0;
  color: #2a2a2a;
  padding: 1rem 2rem;
  border-radius: 8px;
  font-size: 0.95rem;
  font-weight: 500;
  box-shadow: 0 2px 8px rgba(0, 0, 0, 0.12);
  opacity: 0;
  transition: opacity 0.3s ease;
  pointer-events: none;
  z-index: 1000;
}

.toast.show {
  opacity: 1;
}
</style>

<!-- Hero 区域 -->
<div class="hero">
  <h1>YouTube 转录合集</h1>
  <p class="hero-subtitle">每日更新 10+ 优质频道的 AI 转录文稿</p>
  <a href="javascript:void(0);" class="rss-link" id="rss-button">🔔 订阅 RSS</a>
</div>

<!-- Toast 提示 -->
<div class="toast" id="toast">已复制 RSS 订阅源</div>

<!-- 订阅频道筛选 -->
<div class="channel-filters-wrapper">
  <h3 class="channel-filters-title">已包含频道:</h3>
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
</div>

<!-- 转录文章列表 -->
<div id="articles-list">
<h3 class="articles-section-title">已转录文稿</h3>

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
  // RSS 复制功能
  const rssButton = document.getElementById('rss-button');
  const toast = document.getElementById('toast');
  const rssUrl = '{{ site.url }}{{ site.baseurl }}/feed.xml';

  rssButton.addEventListener('click', function(e) {
    e.preventDefault();

    // 复制RSS链接到剪贴板
    navigator.clipboard.writeText(rssUrl).then(function() {
      // 显示toast
      toast.classList.add('show');

      // 2秒后隐藏toast
      setTimeout(function() {
        toast.classList.remove('show');
      }, 2000);
    }).catch(function(err) {
      console.error('复制失败:', err);
    });
  });

  // 频道筛选功能
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
