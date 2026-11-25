---
layout: default
title: 常见问题
description: Telegram 注册常见问题汇总：收不到验证码、登录受限、账号异常等问题的排查与处理方法。
keywords: Telegram常见问题,纸飞机常见问题,Telegram账号常见问题,TG常见问题
permalink: /categories/faq/
---

<section class="page-hero">
  <p class="hero-kicker">分类</p>
  <h1>常见问题</h1>
  <p>Telegram 注册常见问题汇总：收不到验证码、登录受限、账号异常等问题的排查与处理方法。</p>
</section>

<div class="post-list">
  {% assign cat_posts = site.posts | where: "category", "常见问题" %}
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
