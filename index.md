---
layout: default
title: Daily AI News
---

# Hello, AI!

Welcome to my AI News website NOVEMBER.

Check out my [first blog post](./_posts/2024-09-29-and-so-it-begins.md)!

<ul>
  {% for post in site.posts %}
    <li>
      <h2><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h2>
      <p>{{ post.excerpt | truncatewords: 30 }}</p>
      <small>Posted on {{ post.date | date: "%B %d, %Y" }}</small>
    </li>
  {% endfor %}
</ul>