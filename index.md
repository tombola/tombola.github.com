---
layout: page
title: Blog
tagline: ""
published: true
---

{% for post in site.posts %}

  <article class="unit-article layout-post">
  	<h2>{{ post.title }}</h2>
      <!--<span class="glyphicon glyphicon-tag">{{ post.category }}</span>-->
      <p>{{ page.date | date: "%-d %B %Y" }}</p>
      
      <div class="unit-inner unit-article-inner">
          <div class="content">
              <div class="bd">
                  <div class="entry-content">
                      {{ post.content }}
                  </div><!-- entry-content -->
              </div><!-- bd -->
          </div><!-- content -->
      </div><!-- unit-inner -->
  </article>

{% endfor %}