---
layout: main
---

### Arsip Blog
---

<ul>
{% for Berita in site.category %}
{% for post in Berita[1] %}
<li><span>{{ post.date | date_to_string }}</span> - <a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a>
{{ post.excerpt }}</li>
{% endfor %}
{% endfor %}
</ul>

<ul>
{% for Kajian in site.category %}
{% for post in Kajian[1] %}
<li><span>{{ post.date | date_to_string }}</span> - <a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a>
{{ post.excerpt }}</li>
{% endfor %}
{% endfor %}
</ul>
