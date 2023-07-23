---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: home

carousels:
  - images: 
    - image: /assets/img/mary-brush.jpg
    - image: /assets/img/pigment.jpg
    - image: /assets/img/marble.jpg
---

<ul>
{% for post in site.posts %}
    <li><a href="{{post.url}}">{{post.title}}</a></li>
{% endfor %}
</ul>