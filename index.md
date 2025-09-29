---
layout: custom
title: Posts
---

## Latest Posts

- Total posts: {{ site.posts | size }}
- Paginator exists? {% if paginator %}Yes{% else %}No{% endif %}

{% for post in site.posts %}

- [{{ post.title }}]({{ post.url }})
{% endfor %}
