---
layout: custom
title: Categories
permalink: /categories/
---

## Browse by Category

{% for category in site.categories %}

## {{ category[0] }}

{% for post in category[1] %}

- [{{ post.title }}]({{ post.url | relative_url }})  
  _{{ post.date | date: "%B %d, %Y" }}_

{% endfor %}

{% endfor %}
