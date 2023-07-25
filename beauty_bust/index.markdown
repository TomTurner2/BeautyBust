---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: home

carousels:
  - images: 
    - image: /brushbust/
    - image: /bumblast/
    - image: /fashionfail/
---

<style> 

.article
{
  background-position: 25% 75%;
}

.article-card
{
  background-color: rgba(255, 255,255, 0.95);
  height: 173px;
  width: 319px;
  margin: auto;
  margin-top: 200px;
}

.article-card-title
{
    font-family: 'Playfair Display', serif;
    font-style: italic;
    text-align: center;
    font-size: 30;
    width: 100%;
    translate: 0px 15px;
}

.article-card-summary
{
  font-family: 'Source Sans 3', sans-serif;
  font-size: 14;
  text-align: center;
  width: 100%;
  translate: 0px -10px;
}

.article_button__read_now
{
  background-color: #000000;
  width: 133px;
  height: 38px;
  margin: auto;
  transform: translate(0%, -15px);
}

.article_button__read_now:hover {
  background-color: #333;
}

.article_read_now
{
  text-align: center;
  text-decoration: none;
  color: white;
  font-family: 'Source Sans 3', sans-serif;
  font-size: 14;
  line-height: 40px;
}

</style>

<div class="grid-container">
{% for post in site.posts %}
    <div class="grid-item article" style="background-image: url('/assets/img/{{ post.image }}');">
      <div class = "article-card">
        <p class = "article-card-title">{{post.title}}</p>
        <p class = "article-card-summary">{{post.summary}}</p>
        <a style= "text-decoration: none;" href="{{ post.url }}">
          <div class="article_button__read_now">
            <p class="article_read_now" >READ NOW</p>
          </div>
        </a>
      </div>
    </div>
{% endfor %}
</div>