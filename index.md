---
layout: default
title: hopenstock
---


<section>
  {% for post in site.posts do %}
  <article>
  	<div class="title">
  		<h1>
    		<a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a>
    	</h1>
    	<span class="date">{{ post.date | date_to_long_string }}</span>
    </div>
    {{ post.content }}
  	
  </article>
  {% endfor %}
</section>

