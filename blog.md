---
layout: main
---

### Arsip Blog
---

<ul>
  {% for post in site.category[Berita] %}
    <li><span>{{ post.date | date_to_string }}</span> - <a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a>
    {{ post.excerpt }}</li>
  {% endfor %}
</ul>

<ul>
  {% for post in site.category[Kajian] %}
    <li><span>{{ post.date | date_to_string }}</span> - <a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a>
    {{ post.excerpt }}</li>
  {% endfor %}
</ul>
