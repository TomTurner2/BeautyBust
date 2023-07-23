---
layout: "page"
title: Lifestyle
permalink: /lifestyle/
navbar: true
---

<ul>
   {% for post in site.categories["fitness"] %}
    <li>
      <a href="{{ post.url }}">
        {{ post.title }}
      </a>
      - <time datetime="{{ post.date | date: "%Y-%m-%d" }}">{{ post.date | date_to_long_string }}</time>
    </li>
  {% endfor %}
</ul>