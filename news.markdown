---
layout: base
---

{% for post in site.categories.en %}
<div class="post-container">
	<div class="entry-title">
		<h2><a href="{{post.url}}">{{ post.title }}</a></h2>
	</div>
	<div class="entry-meta">
		Published by {{post.author}} at {{post.date | date: '%d %B %Y'}}
	</div>
	<div class="entry-content">
		{{ post.content }}
	</div>
</div>
{% endfor %}
