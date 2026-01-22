---
layout: page
title: Arsip
---

<section>
{% assign current_year = "" %}

{% for post in site.posts %}
  {% capture post_year %}{{ post.date | date: "%Y" }}{% endcapture %}

  {% if post_year != current_year %}
    {% unless forloop.first %}
      </ul>
    {% endunless %}

    <h1>{{ post_year }}</h1>
    
    <ul class="archive-list">
    
    {% assign current_year = post_year %}
  {% endif %}

  <li class="archive-item">
      <div class="item-content">
          <span class="archive-date">{{ post.date | date: "%d %b" }}</span>
          <a href="{{ post.url | relative_url }}" class="archive-title">{{ post.title }}</a>
      </div>
  </li>

  {% if forloop.last %}
    </ul>
  {% endif %}

{% endfor %}
</section>