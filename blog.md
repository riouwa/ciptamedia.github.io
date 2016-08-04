---
layout: main
---

### Arsip Blog
---

<ul>
  {% for Berita in site.category %}
    <span id="{{ Berita[0] }}" class="Berita">{{ Berita[0] }}</span>
    {% for post in Berita[1] %}
      <li><span>{{ post.date | date_to_string }}</span> - <a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a>
      {{ post.excerpt }}</li>
    {% endfor %}
  {% endfor %}
</ul>

<ul>
  {% for Kajian in site.category %}
    <span id="{{ Kajian[0] }}" class="Kajian">{{ Kajian[0] }}</span>
    {% for post in Kajian[1] %}
      <li><span>{{ post.date | date_to_string }}</span> - <a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a>
      {{ post.excerpt }}</li>
    {% endfor %}
  {% endfor %}
</ul>
