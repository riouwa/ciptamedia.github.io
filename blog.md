---
layout: main
---

### Arsip Blog
---

<ul>
{% for Berita in site.category %}
<li><span>{{ post.date | date_to_string }}</span> - <a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a>
{{ post.excerpt }}</li>
{% endfor %}
</ul>
