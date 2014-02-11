---
layout: page
title: Blog
tagline: ""
published: true
---

{% for post in site.posts %}

  <article class="unit-article layout-post">
  	<h2><a href="{{ post.url }}">{{ post.title }}</a></h2>
      <!--<span class="glyphicon glyphicon-tag">{{ post.category }}</span>-->
      <p><em><time datetime="{{ post.date | date: "%Y-%m-%d" }}">{{ post.date | date: "%-d %B %Y" }}</time></em></p>
      {{ post.content }}
  </article>

{% endfor %}