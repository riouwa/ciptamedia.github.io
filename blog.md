---
layout: main
---

### Arsip Blog
---

<div class="btn-group">
  <button type="button" class="btn btn-danger">Kategori</button>
  <button type="button" class="btn btn-danger dropdown-toggle" data-toggle="dropdown" aria-expanded="false">
    <span class="caret"></span>
    <span class="sr-only">Toggle Dropdown</span>
  </button>
  <ul class="dropdown-menu" role="menu">
    <li><a href="#berita" id="filterProblems-all">Berita</a></li>
    <li><a href="#kajian" id="filterProblems-solved">Kajian</a></li>
  </ul>
</div>

<div class="content">
  <div class="tab-content">
    <div class="tab-pane active" id="berita">
      <ul>
        {% for post in site.categories.Berita %}
          <li><span>{{ post.date | date_to_string }}</span> - <a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a>
          {{ post.excerpt }}</li>
        {% endfor %}
      </ul>
    </div>
    <div class="tab-pane active" id="berita">
      <ul>
        {% for post in site.categories.Kajian %}
          <li><span>{{ post.date | date_to_string }}</span> - <a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a>
          {{ post.excerpt }}</li>
        {% endfor %}
      </ul>
    </div>
  </div>
</div>
