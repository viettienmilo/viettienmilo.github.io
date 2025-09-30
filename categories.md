---
layout: custom
title: MIS
permalink: /categories/mis/
---

## Posts in MIS

{% assign posts_in_cat = site.posts | where: "category", "MIS" %}
{% for post in posts_in_cat %}

- [{{ post.title }}]({{ post.url | relative_url }})
  _{{ post.date | date: "%B %d, %Y" }}_
{% endfor %}
