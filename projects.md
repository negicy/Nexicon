---
layout: page
title: Projects
permalink: /projects/
---


<ul>
  {% for post in site.posts %}
    {% if post.category == "project" %}
    <li>
      <h2><a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a></h2>
      {{ post.excerpt }}
    </li>
    {% endif %}
  {% endfor %}
</ul>