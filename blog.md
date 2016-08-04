---
layout: main
---

### Arsip Blog
---

<ul class="nav nav-pills nav-pills-danger" role="tablist">
	<li>
		<a href="#dashboard" role="tab" data-toggle="tab">
			<i class="material-icons">dashboard</i>
			Dashboard
		</a>
	</li>
	<li class="active">
		<a href="#schedule" role="tab" data-toggle="tab">
			<i class="material-icons">schedule</i>
			Schedule
		</a>
	</li>
	<li>
		<a href="#tasks" role="tab" data-toggle="tab">
			<i class="material-icons">list</i>
			Tasks
		</a>
	</li>
</ul>

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
