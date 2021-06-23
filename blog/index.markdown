---
layout: default
title: Sodhinchu's blog
---
	<h1>{{ page.title }}</h1>
	<ul>
	  {% for post in site.posts %}
	    <li>
			<a href="{{ post.url }}" title="{{ post.title }}"</a>
			{{ post.excerpt }}
		</li>
	  {% endfor %}
	</ul>
