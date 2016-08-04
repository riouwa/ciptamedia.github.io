---
layout: main
---

## Arsip Berita_test
---
<ul>
{% for post in site.posts %}
<li><span>{{ post.date | date_to_string }}</span> - <a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a>
</br>{{ post.excerpt }} <a href="{{ site.baseurl }}{{ post.url }}">baca lagi...</a></li>
{% endfor %}
</ul>
