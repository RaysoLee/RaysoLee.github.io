---
layout: page
title: Blog
permalink: /Blog/
---

<div class="home">
  <h1 class="page-heading">{{ site.title }}</h1>
  <ul class="post-list">
    {% for post in site.posts %}
      <li class="lightSpeedIn wow">
        <span class="post-meta">{{ post.date | date: "%b %-d, %Y" }}</span>

        <h2>
          <a class="post-link" href="{{ post.url | prepend: site.baseurl }}">{{ post.title | escape }}</a>
        </h2>
      </li>
    {% endfor %}
  </ul>
  <p class="rss-subscribe">subscribe <a href="{{ "/feed.xml" | prepend: site.baseurl }}">via RSS</a></p>
</div>