---
layout: main
---

### Arsip Blog
---

<div class="btn-group">
  <button type="button" class="btn btn-danger dropdown-toggle" data-toggle="dropdown" aria-expanded="false">Kategori
    <span class="caret"></span>
    <span class="sr-only">Toggle Dropdown</span>
  </button>
  <ul class="dropdown-menu" role="menu">
    <li><a href="#berita" data-toggle="tab">Berita</a></li>
    <li><a href="#kajian" data-toggle="tab">Kajian</a></li>
    <li><a href="#all" data-toggle="tab">Semua</a></li>
  </ul>
</div>

<div class="content">
  <div class="tab-content">
    <div class="tab-pane active" id="all">
      <ul>
        {% for post in site.posts %}
          <li><h4><a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a></h4>
          <span>{{ post.date | date_to_string }}</span>
          {{ post.excerpt }}</li>
        {% endfor %}
      </ul>
    </div>
    <div class="tab-pane" id="berita">
      <ul>
        {% for post in site.categories.Berita %}
          <li><h4><a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a></h4>
          <span>{{ post.date | date_to_string }}</span>
          {{ post.excerpt }}</li>
        {% endfor %}
      </ul>
    </div>
    <div class="tab-pane" id="kajian">
      <ul>
        {% for post in site.categories.Kajian %}
          <li><h4><a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a></h4>
          <span>{{ post.date | date_to_string }}</span>
          {{ post.excerpt }}</li>
        {% endfor %}
      </ul>
    </div>
  </div>
</div>
