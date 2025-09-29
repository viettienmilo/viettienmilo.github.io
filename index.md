---
layout: custom
title: Posts
---

## Latest Posts

{% for post in site.posts limit:5 %}

- [{{ post.title }}]({{ post.url | relative_url }})  
  _{{ post.date | date: "%B %d, %Y" }}_
  
{% endfor %}

---

[View all posts]({{ '/archive/' | relative_url }})
