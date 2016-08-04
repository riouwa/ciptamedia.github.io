---
layout: main
---

### Arsip Blog
---

<ul>
  {% for post in site.categories.Berita %}
    <li><span>{{ post.date | date_to_string }}</span> - <a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a>
    {{ post.excerpt }}</li>
  {% endfor %}
</ul>

<ul>
  {% for post in site.categories.Kajian %}
    <li><span>{{ post.date | date_to_string }}</span> - <a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a>
    {{ post.excerpt }}</li>
  {% endfor %}
</ul>
