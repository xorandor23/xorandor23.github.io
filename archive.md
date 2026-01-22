---
layout: page
title: Arsip
---


{% if site.posts[0] %}
{% capture currentyear %}{{ 'now' | date: "%Y" }}{% endcapture %}
{% if currentyear == firstpostyear %}
    <h1>Tahun ini</h1>
{% else %}  
    <h1>{{ firstpostyear }}</h1>
{% endif %}


{%for post in site.posts %}
  {% unless post.next %}
      <ul class="archive-list">
  {% else %}
    {% capture year %}{{ post.date | date: '%Y' }}{% endcapture %}
    {% capture nyear %}{{ post.next.date | date: '%Y' }}{% endcapture %}
    {% if year != nyear %}
      </ul>
      <h1>{{ post.date | date: '%Y' }}</h1>
      <ul class="archive-list">
    {% endif %}
  {% endunless %}
      <li class="archive-item">
          <div class="item-content">
              <span class="archive-date">{{ post.date | date:"%d %b" }}</span>
              <a href="#" class="archive-title">{{ post.title }}</a>
          </div>
      </li>
{% endfor %}
</ul>

{% endif %}
