---
layout: "page"
title: All
permalink: /all/
navbar: true
---

{% include style.html %}
<h1>All</h1>
{% include followMe.html %}


<div class="grid-container">
  {% for p in site.posts %}
      {% include articleCard.html image = p.image title = p.title summary = p.summary url = p.url %}
  {% endfor %}
</div>