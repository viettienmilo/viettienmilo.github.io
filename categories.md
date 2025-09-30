---
layout: custom
title: Categories
permalink: /categories/
---


{% assign grouped = site.posts | group_by: "category" %}
{% for subject in grouped %}

## <span class="category-title">{{ subject.name }}</span>

  {% assign subgroups = subject.items | group_by: "subcategory" %}
  {% for chapter in subgroups %}

### <span class="subcategory-title">{{ chapter.name }}</span>

  {% for post in chapter.items %}

- [{{ post.title }}]({{ post.url | relative_url }})
    _{{ post.date | date: "%B %d, %Y" }}_

  {% endfor %}

  {% endfor %}

{% endfor %}
