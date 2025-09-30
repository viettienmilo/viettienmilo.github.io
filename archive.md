---
layout: custom
title: Archive
permalink: /archive/
---

## All Posts

{% for post in site.posts %}

- [{{ post.title }}]({{ post.url | relative_url }})  
  _{{ post.date | date: "%B %d, %Y" }}_

{% endfor %}
