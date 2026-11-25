---
layout: default
title: 使用教程
description: Telegram 账号使用教程：接码号说明、登录后安全设置、账号养护与防封实务。
keywords: Telegram使用教程,纸飞机使用教程,Telegram账号使用教程,TG使用教程
permalink: /categories/use-guide/
---

<section class="page-hero">
  <p class="hero-kicker">分类</p>
  <h1>使用教程</h1>
  <p>Telegram 账号使用教程：接码号说明、登录后安全设置、账号养护与防封实务。</p>
</section>

<div class="post-list">
  {% assign cat_posts = site.posts | where: "category", "使用教程" %}
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
