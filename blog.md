---
layout: main
---

## Arsip Berita
---
<ul>
{% for post in site.posts %}
<li><span>{{ post.date | date_to_string }}</span> - <a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a>
{{ post.excerpt }}</li>
{% endfor %}
</ul>
