---
layout: main
---

### Arsip Blog
---

<ul>
{% for Berita in site.categories %}
<li><span>{{ post.date | date_to_string }}</span> - <a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a>
{{ post.excerpt }}</li>
{% endfor %}
</ul>

<ul>
{% for Kajian in site.categories %}
<li><span>{{ post.date | date_to_string }}</span> - <a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a>
{{ post.excerpt }}</li>
{% endfor %}
</ul>
