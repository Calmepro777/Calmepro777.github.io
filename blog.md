---
layout: page
title: Blog
permalink: /blog/
---

Thoughts on investing, Cardano, and why most of what you've been told about crypto is wrong.

{% for post in site.posts %}
### [{{ post.title }}]({{ post.url | relative_url }})
<small>{{ post.date | date: "%B %d, %Y" }} · {{ post.categories | join: ", " }}</small>

{{ post.excerpt | strip_html | truncatewords: 40 }}

---
{% endfor %}
