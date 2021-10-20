---
layout: default
title: Sodhinchu's blog
---
<div class="posts">
  {% for post in site.posts %}
    <article class="post">

      <h1><a href="{{ site.baseurl }}{{ post.url }}">
        {{ post.title }}</a>
      </h1>

      <div class="entry">
        {{ post.excerpt }}
      </div>
      
      {% if post.categories %} | 
        {% for category in post.categories %}
          <a href="{{ site.baseurl }}{{ site.category_page }}#{{ category | slugify }}" class="post-tag">{{ category }}</a>
        {% endfor %}
    {% endif %}

      {% if post.excerpt != post.content %}
        <a href="#{{ post.url }}">Read more</a>
      {% endif %}
    </article>
  {% endfor %}
</div>
