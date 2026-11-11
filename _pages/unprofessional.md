---
title: "Unprofessional stuff"
permalink: /unprofessional/
layout: single
classes: unprofessional-archive
---

{% assign posts = site.categories.unprofessional | sort: "date" | reverse %}

<ul class="unprofessional-post-list">
{% for post in posts %}
  <li>
    <a href="{{ post.url | relative_url }}">{{ post.title | escape }}</a>
  </li>
{% endfor %}
</ul>
