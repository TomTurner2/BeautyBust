---
layout: "page"
title: Fitness
permalink: /fitness/
navbar: true
---

{% include style.html %}
<h1>Fitness</h1>
{% include followMe.html %}


<div class="grid-container">
{% for p in site.categories["fitness"] %}
    {% include articleCard.html image = p.image title = p.title summary = p.summary url = p.url %}
{% endfor %}
</div>