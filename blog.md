---
layout: page
title: Prescriptions
navbar: display
navbar_display: Blog
permalink: /blog/
heading: Recent Posts
---

<h2 class="page-heading">{{page.heading}}</h2>

<ul class="post-list">
  {% for post in site.posts %}
    <li>
      <span class="post-meta">{{ post.date | date: "%b %-d, %Y" }}</span>

      <h3>
        <a class="post-link" href="{{ post.url | relative_url }}">{{ post.title | escape }}</a>
      </h3>
    </li>
  {% endfor %}
</ul>
