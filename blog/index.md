---
layout: default
title: Sodhinchu's blog
category: Dev
tags: [web, jekyll]
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
      
      {% if post.tags %} | 
        {% for tag in post.tags %}
          <a href="{{ site.baseurl }}{{ site.tag_page }}#{{ tag | slugify }}" class="post-tag">{{ tag }}</a>
        {% endfor %}
    {% endif %}

      {% if post.excerpt != post.content %}
        <a href="{{ post.url }}">Read more</a>
      {% endif %}
    </article>
  {% endfor %}
</div>
