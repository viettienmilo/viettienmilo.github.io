---
layout: custom
title: Posts
---

## Latest Posts

{% for post in paginator.posts %}

- [{{ post.title }}]({{ post.url }})  
  _{{ post.date | date: "%B %d, %Y" }}_
{% endfor %}

<!-- - Total posts: {{ site.posts | size }}
- Paginator exists? {% if paginator %}Yes{% else %}No{% endif %}

{% for post in site.posts %}

- [{{ post.title }}]({{ post.url }})
{% endfor %} -->
