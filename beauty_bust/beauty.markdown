---
layout: "page"
title: Beauty
permalink: /beauty/
navbar: true
---

<ul>
   {% for post in site.categories["beauty"] %}
    <li>
      <a href="{{ post.url }}">
        {{ post.title }}
      </a>
      - <time datetime="{{ post.date | date: "%Y-%m-%d" }}">{{ post.date | date_to_long_string }}</time>
    </li>
  {% endfor %}
</ul>
