---
layout: page
title: Raspberry Pi
permalink: /raspi/
---

**Raspberry Pi posts:**
<ul>
  {% for post in site.categories.raspi %}
    <li>
      <a href="{{ post.url | prepend: site.github.url }}">{{ post.title }}</a>
      {{ post.excerpt }}
    </li>
  {% endfor %}
</ul>
