---
layout: main
title: Cipta Media Blog Archieve
---

## Arsip Berita
---
<ul>
{% for post in site.posts %}
<li><span>{{ post.date | date_to_string }}</span> &raquo; <a href="{{ post.url }}">{{ post.title }}</a>{{ post.url }}</li>
{% endfor %}
</ul>
