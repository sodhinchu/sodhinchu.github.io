---
layout: feed
---
<?xml version="1.0" encoding="utf-8"?>
<feed xmlns="http://www.w3.org/2005/Atom">

	<title>Sodhinchu's Blog</title>
	<link href="http://sodhinchu.github.io/blog/atom.xml" rel="self"/>
	<link href="http://sodhinchu.github.io/blog"/>
	<updated>{{ site.time | date_to_xmlschema }}</updated>
	<id>http://sodhinchu.github.io/blog</id>
	<author>
		<name>Sodhinchu</name>
		<email>sodhinchu@gmail.com</email>
	</author>

	{% for tag in tags %}
		<h2 id="{{ tag | slugify }}">{{ tag }}</h2>
		<ul>
			{% for post in site.posts %}
				<entry>
					<title>{{ post.title }}</title>
					<link href="http://sodhinchu.github.io{{ post.url }}"/>
					<updated>{{ post.date | date_to_xmlschema }}</updated>
					<id>http://sodhinchu.github.io{{ post.id }}</id>
					<content type="html">{{ post.content | xml_escape }}</content>
				</entry>
			{% endfor %}
		</ul>
	{% endfor %}		

</feed>
