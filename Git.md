---
layout: page
title: Git
permalink: /git/
---

**Git posts:**
<ul>
  {% for post in site.categories.git %}
    <li>
      <a href="{{ post.url | prepend: site.github.url }}">{{ post.title }}</a>
      {{ post.excerpt }}
    </li>
  {% endfor %}
</ul>
