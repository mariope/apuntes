---
layout: page
title: R
permalink: /r/
---

**R posts:**
<ul>
  {% for post in site.categories.r %}
    <li>
      <a href="{{ post.url | prepend: site.github.url }}">{{ post.title }}</a>
      {{ post.excerpt }}
    </li>
  {% endfor %}
</ul>
