---
layout: home
title: YouTube 转录合集
---

<div style="text-align: center; padding: 1.5rem 0 1rem;">
  <p style="font-size: 1rem; color: #666; margin-bottom: 1rem;">
    每日更新 10+ 优质频道的 AI 转录文稿
    <a href="{{ site.baseurl }}/feed.xml" style="margin-left: 0.5rem; text-decoration: none; color: #667eea; font-weight: 500;">🔔 订阅RSS</a>
  </p>
</div>

<!-- 订阅频道筛选 -->
<div style="margin: 1.5rem 0; padding: 1rem; background: #f7fafc; border-radius: 8px;">
  <div style="display: grid; grid-template-columns: repeat(5, 1fr); gap: 0.6rem;">
    <button class="channel-filter active" data-channel="all" style="padding: 0.5rem; background: #667eea; color: white; border: none; border-radius: 4px; cursor: pointer; font-size: 0.85rem;">全部</button>
    <button class="channel-filter" data-channel="Peter Yang" style="padding: 0.5rem; background: white; border: 1px solid #e1e8ed; border-radius: 4px; cursor: pointer; font-size: 0.85rem;">Peter Yang</button>
    <button class="channel-filter" data-channel="Dwarkesh Patel" style="padding: 0.5rem; background: white; border: 1px solid #e1e8ed; border-radius: 4px; cursor: pointer; font-size: 0.85rem;">Dwarkesh Patel</button>
    <button class="channel-filter" data-channel="Lenny's Podcast" style="padding: 0.5rem; background: white; border: 1px solid #e1e8ed; border-radius: 4px; cursor: pointer; font-size: 0.85rem;">Lenny's Podcast</button>
    <button class="channel-filter" data-channel="The MAD Podcast with Matt Turck" style="padding: 0.5rem; background: white; border: 1px solid #e1e8ed; border-radius: 4px; cursor: pointer; font-size: 0.85rem;">Data-Driven NYC</button>
    <button class="channel-filter" data-channel="Greg Isenberg" style="padding: 0.5rem; background: white; border: 1px solid #e1e8ed; border-radius: 4px; cursor: pointer; font-size: 0.85rem;">Greg Isenberg</button>
    <button class="channel-filter" data-channel="Dialectic Podcast with Jackson Dahl" style="padding: 0.5rem; background: white; border: 1px solid #e1e8ed; border-radius: 4px; cursor: pointer; font-size: 0.85rem;">Dialectic</button>
    <button class="channel-filter" data-channel="David Perell" style="padding: 0.5rem; background: white; border: 1px solid #e1e8ed; border-radius: 4px; cursor: pointer; font-size: 0.85rem;">David Perell</button>
    <button class="channel-filter" data-channel="The Knowledge Project Podcast" style="padding: 0.5rem; background: white; border: 1px solid #e1e8ed; border-radius: 4px; cursor: pointer; font-size: 0.85rem;">TKP Podcast</button>
    <button class="channel-filter" data-channel="Every" style="padding: 0.5rem; background: white; border: 1px solid #e1e8ed; border-radius: 4px; cursor: pointer; font-size: 0.85rem;">Every</button>
    <button class="channel-filter" data-channel="Y Combinator" style="padding: 0.5rem; background: white; border: 1px solid #e1e8ed; border-radius: 4px; cursor: pointer; font-size: 0.85rem;">Y Combinator</button>
  </div>
</div>

<!-- 转录文章列表 -->
<div id="articles-list" style="margin: 2rem 0;">
{% assign all_pages = site.html_pages | where_exp: "page", "page.title != nil" | where_exp: "page", "page.channel != nil" | sort: 'date' | reverse %}

{% for page in all_pages limit:20 %}
<div class="article-card" data-channel="{{ page.channel }}" style="padding: 1rem; margin-bottom: 0.8rem; border: 1px solid #e1e8ed; border-radius: 6px; background: white;">
  <div style="display: flex; justify-content: space-between; align-items: baseline; margin-bottom: 0.3rem;">
    <h3 style="margin: 0; font-size: 1.1rem; font-weight: 500;">
      <a href="{{ site.baseurl }}{{ page.url }}" style="text-decoration: none; color: #1a1a1a;">{{ page.title }}</a>
    </h3>
    <span style="font-size: 0.85rem; color: #999; white-space: nowrap; margin-left: 1rem;">{{ page.date | date: "%Y-%m-%d" }}</span>
  </div>
  <div style="font-size: 0.85rem; color: #666;">
    📺 {{ page.channel }}
  </div>
</div>
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
          btn.style.background = '#667eea';
          btn.style.color = 'white';
          btn.style.border = 'none';
        } else {
          btn.classList.remove('active');
          btn.style.background = 'white';
          btn.style.color = '#1a1a1a';
          btn.style.border = '1px solid #e1e8ed';
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
<div style="text-align: center; padding: 2rem 0; margin-top: 3rem; border-top: 1px solid #e1e8ed; color: #999; font-size: 0.85rem;">
  <p style="margin: 0;">
    <a href="#about" style="color: #666; text-decoration: none;">关于本站</a>
    <span style="margin: 0 0.5rem;">|</span>
    <a href="{{ site.baseurl }}/feed.xml" style="color: #666; text-decoration: none;">RSS订阅</a>
    <span style="margin: 0 0.5rem;">|</span>
    <span>Powered by <a href="https://deepmind.google/technologies/gemini/" target="_blank" style="color: #667eea; text-decoration: none;">Gemini 2.5</a> & <a href="https://jekyllrb.com/" target="_blank" style="color: #667eea; text-decoration: none;">Jekyll</a></span>
  </p>
</div>
