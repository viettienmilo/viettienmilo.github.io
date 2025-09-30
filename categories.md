---
layout: custom
title: Categories
permalink: /categories/
---

## Browse by Category

{% assign grouped = site.posts | group_by: "category" %}
{% for subject in grouped %}

### {{ subject.name }}

  {% assign subgroups = subject.items | group_by: "subcategory" %}
  {% for chapter in subgroups %}

#### {{ chapter.name }}

  {% for post in chapter.items %}

- [{{ post.title }}]({{ post.url | relative_url }})
    _{{ post.date | date: "%B %d, %Y" }}_

  {% endfor %}

  {% endfor %}

{% endfor %}
