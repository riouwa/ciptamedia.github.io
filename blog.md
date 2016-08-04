---
layout: main
---

### Arsip Blog
---

<ul class="nav nav-pills nav-pills-danger" role="tablist">
	<li>
		<a href="#berita" role="tab" data-toggle="tab">
			<i class="material-icons">dashboard</i>
			Berita
		</a>
	</li>
	<li class="active">
		<a href="#kajian" role="tab" data-toggle="tab">
			<i class="material-icons">schedule</i>
			Kajian
		</a>
	</li>
</ul>

<div class="tab-pane active" id="berita">
<ul>
  {% for post in site.categories.Berita %}
    <li><span>{{ post.date | date_to_string }}</span> - <a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a>
    {{ post.excerpt }}</li>
  {% endfor %}
</ul>
</div>

<ul>
  {% for post in site.categories.Kajian %}
    <li><span>{{ post.date | date_to_string }}</span> - <a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a>
    {{ post.excerpt }}</li>
  {% endfor %}
</ul>
