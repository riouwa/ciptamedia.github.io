---
layout: main
---

## Arsip Berita
---
<ul>
{% for post in site.posts %}
<li><span>{{ post.date | date_to_string }}</span> &raquo; <a href="{{ page.url }}">{{ post.title }}</a></br>{{ post.excerpt }}</li>
{% endfor %}
</ul>
