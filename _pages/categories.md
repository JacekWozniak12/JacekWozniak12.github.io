---
layout: page
permalink: /categories/
title: Categories
---


<div id="archives">
{% for category in site.categories %}
  <div class="archive-group">
    {% capture category_name %}{{ category | first }}{% endcapture %}
    <div id="{{ category_name | slugize }}"></div>
    <p></p>
    
    <a name="{{ category_name | slugize }}" id = "{{ category_name | slugize }}" class="-group-header-hs"><h3 class="category-head">{{ category_name }}</h3>
    </a>
    <div class="article-group close" id="{{category_name}}">
    {% for post in site.categories[category_name] %}
    <article class="archive-item">
      <a href="{{ site.baseurl }}{{ post.url }}">{% if post.title and post.title != "" %}{{post.title}}{% else %}{{post.excerpt |strip_html}}{%endif%}</a>
    </article>
    {% endfor %}
    </div>
  </div>
{% endfor %}
</div>
