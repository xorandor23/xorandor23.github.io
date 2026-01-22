---
layout: page
title: Arsip
---

{% capture current_year %}{{ 'now' | date: "%Y" }}{% endcapture %}

{% for post in site.posts %}
  {% capture post_year %}{{ post.date | date: '%Y' }}{% endcapture %}

  {% if post_year != year %}
    
    {% unless forloop.first %}</ul>{% endunless %}

    {% if post_year == current_year %}
      <h1>Tahun Ini</h1>
    {% else %}
      <h1>{{ post_year }}</h1>
    {% endif %}

    <ul class="archive-list">
    
    {% assign year = post_year %}
  {% endif %}

  <li class="archive-item">
      <div class="item-content">
          <span class="archive-date">{{ post.date | date: "%d %b" }}</span>
          
          <a href="{{ post.url | relative_url }}" class="archive-title">{{ post.title }}</a>
      </div>
  </li>

  {% if forloop.last %}</ul>{% endif %}

{% endfor %}