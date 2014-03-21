---
layout: page
title: Blog
tagline: ""
published: true
---

{% for post in site.posts %}

  <article class="unit-article layout-post">
    <h1><a href="{{ post.url }}">{{ post.title }}</a> {% if post.tagline %} <small>{{post.tagline}}</small>{% endif %}</h1>
      <!--<span class="glyphicon glyphicon-tag">{{ post.category }}</span>-->
      <p class="date"><time datetime="{{ post.date | date: "%Y-%m-%d" }}">{{ post.date | date: "%-d %B %Y" }}</time></p>
      {{ post.content }}
  </article>
  <hr>

{% endfor %}