---
layout: default
title: Lino Grubben
---

<h1 class="page-title">Lino Grubben</h1>
<p class="bio">
  I’m a designer and entrepreneur writing about product, design,
  and what else is on my mind.
</p>

{% for post in site.posts %}
  <div class="post-item">
    <a href="{{ post.url | relative_url }}" class="post-title">
      {{ post.title }}
    </a>
    <p class="post-date">{{ post.date | date_to_string }}</p>
  </div>
{% endfor %}
