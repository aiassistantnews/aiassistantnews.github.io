---
layout: default
title: Daily AI News
---

<!-- # Hello, AI!

Welcome to AI News. Here you'll find the most interesting news about AI in a short and quick to read format. -->

## Blog posts

<!-- Check out my [first blog post](./_posts/2024-09-29-and-so-it-begins.md)! -->

{% for post in site.posts %}
<div class="post-content">
<!-- <h2>{{ post.title }}</h2> -->
<p>{{ post.excerpt | strip_html | truncatewords: 50 }}</p>
<a href="{{ post.url | relative_url }}" class="post-link">Go to article...</a>
<small>Posted on {{ post.date | date: "%B %d, %Y" }}</small>
</div>
{% endfor %}
