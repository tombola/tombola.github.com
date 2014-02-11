---
layout: page
title: Hello World
tagline: ""
published: true
---

For non-geeks, [hello world](http://en.wikipedia.org/wiki/Hello_world_program) is where every bit of software, or assay into new coding language starts.

<ul class="posts">
{% for post in site.posts limit: 20 %}
  <div class="post_info">
    <li>
         <a href="{{ post.url }}">{{ post.title }}</a> 
         <span>({{ post.date | date:"%Y-%m-%d" }})</span>
    </li>
    </div>
  {% endfor %}
</ul>