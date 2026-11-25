---
layout: default
title: 账号选购
description: Telegram 新号、老号与成品号的区别对比，以及账号选购时的注意事项与风险识别方法。
keywords: Telegram账号选购,纸飞机账号选购,Telegram账号账号选购,TG账号选购
permalink: /categories/account/
---

<section class="page-hero">
  <p class="hero-kicker">分类</p>
  <h1>账号选购</h1>
  <p>Telegram 新号、老号与成品号的区别对比，以及账号选购时的注意事项与风险识别方法。</p>
</section>

<div class="post-list">
  {% assign cat_posts = site.posts | where: "category", "账号选购" %}
  {% for post in cat_posts %}
  <article class="post-row">
    <a href="{{ post.url }}" class="row-img placeholder" aria-hidden="true">
      {% case post.category %}
      {% when '使用教程' %}📖{% when '账号选购' %}🔑{% when '常见问题' %}❓{% else %}🚀{% endcase %}
    </a>
    <div class="row-body">
      <div class="row-meta">
        <time>{{ post.date | date: '%Y-%m-%d' }}</time>
        <span class="cat-tag">{{ post.category }}</span>
      </div>
      <h2><a href="{{ post.url }}">{{ post.title }}</a></h2>
      <p>{{ post.description }}</p>
    </div>
  </article>
  {% endfor %}
</div>
