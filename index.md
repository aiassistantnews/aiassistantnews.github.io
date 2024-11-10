---
layout: default
title: Daily AI News
---

# Hello, AI!

Welcome to my AI News website NOVEMBER.

Check out my [first blog post](./_posts/2024-09-29-and-so-it-begins.md)!

{% for post in site.posts %}
<p>
=-=
## <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
{{ post.excerpt | truncatewords: 30 }}
<small>Posted on {{ post.date | date: "%B %d, %Y" }}</small>
-+-
</p>
{% endfor %}
