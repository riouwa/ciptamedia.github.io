---
layout: main
---

### Arsip Blog
---

<div class="btn-group">
  <button type="button" class="btn btn-danger">Kategori</button>
  <button type="button" class="btn btn-danger dropdown-toggle" data-toggle="dropdown" aria-expanded="false"></button>
  <ul class="dropdown-menu" role="menu">
    <li><a href="#berita" id="filterProblems-all">Berita</a></li>
    <li><a href="#kajian" id="filterProblems-solved">Kajian</a></li>
  </ul>
</div>

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
