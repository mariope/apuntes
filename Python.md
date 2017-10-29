---
layout: page
title: Python
permalink: /python/
---

**Python posts:**
<ul>
  {% for post in site.categories.python %}
    <li>
      <a href="{{ post.url | prepend: site.github.url }}">{{ post.title }}</a>
      {{ post.excerpt }}
    </li>
  {% endfor %}
</ul>
