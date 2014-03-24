---
layout: page
title: edtech ramblings
tagline: ""
published: true
---

{% for post in site.posts %}

  <article class="unit-article layout-post">
    <h2><a href="{{ post.url }}">{{ post.title }}</a> {% if post.tagline %} <small>{{post.tagline}}</small>{% endif %}</h2>
      <!--<span class="glyphicon glyphicon-tag">{{ post.category }}</span>-->
      <p class="date"><time datetime="{{ post.date | date: "%Y-%m-%d" }}">{{ post.date | date: "%-d %B %Y" }}</time></p>
      {{ post.content }}
  </article>
  <hr>

{% endfor %}