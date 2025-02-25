---
layout: default
title: Home
---

{% for post in site.posts %}
  <div class="post-item">
    <a href="{{ post.url | relative_url }}" class="post-title">
      {{ post.title }}
    </a>
    <p class="post-date">{{ post.date | date_to_string }}</p>
  </div>
{% endfor %}
