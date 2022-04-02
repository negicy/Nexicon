---
layout: page
title: Projects
permalink: /projects/
---
現在参加中，または過去に参加したプロジェクト一覧：

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