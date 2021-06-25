---
layout: default
title: Sodhinchu's blog
---
<ul>
  {% for post in site.posts %}
    <li>
      <a href="{{ post.url }}">{{ post.title }}</a>
    </li>
    <div class="entry">
    	{{ post.excerpt }}
    </div>	
    <a href="{{ site.baseurl }}{{ post.url }}" class="read-more">Read More</a>
  {% endfor %}
</ul>
