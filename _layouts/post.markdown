---
layout: default
post: active
---
<h1>{{ page.title }}</h1>
<p class="meta">{{ page.date | date_to_string }}</p>

<div class="post">
  {{ content }}
  
  <!-- Post comments
  <div class="notecomments">
    {% include comments.html %}	 
  </div>   -->
</div>
{% include comments.html %}
