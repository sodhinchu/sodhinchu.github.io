---
layout: default
title: Blog
---

<a role="button" href="#bm1" class="btn btn-primary btn-md">Visual Grounding </a>
<a role="button" href="#bm2" class="btn btn-primary btn-md">Automatic Thesaurus</a>
<a role="button" href="#bm3" class="btn btn-primary btn-md">PhD Application Process</a>

<p>&nbsp;</p>
## Visual Grounding {#bm1}
<p></p>

<div class="posts">
  {% for post in site.posts %}
    <article class="post">

      <h1><a href="{{ site.baseurl }}{{ post.url }}">
        {{ post.title }}</a>
      </h1>

      <div class="entry">
        {{ post.excerpt }}
      </div>
      
      {% if post.excerpt != post.content %}
        <a href="#{{ post.url }}">Read more</a>
      {% endif %}
    </article>
  {% endfor %}
</div>
