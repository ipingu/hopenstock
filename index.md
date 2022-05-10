---
layout: default
title: Latest beer recipes from Hopenstock brewery
---
<section>
  {% for post in site.posts %}
  <article>
  	<div class="title">
  		<h2>
    		<a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a>
    	</h2>
    	<span class="date">{{ post.date | date_to_long_string }}</span>
    </div>
    <div class="indent">
      {{ post.excerpt }}
    </div>
  </article>
  {% endfor %}
</section>

