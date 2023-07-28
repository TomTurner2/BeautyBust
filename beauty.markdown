---
layout: "page"
title: Beauty
permalink: /beauty/
navbar: true
---

{% include style.html %}
<h1>Beauty</h1>
{% include followMe.html %}


<div class="grid-container">
{% for p in site.categories["beauty"] %}
    {% include articleCard.html image = p.image title = p.title summary = p.summary url = p.url x=p.imgX y=p.imgY scaleX= p.imgScaleX scaleY= p.imgScaleY%}
{% endfor %}
</div>