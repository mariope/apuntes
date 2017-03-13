---
layout: page
title: Raspberry Pi
permalink: /raspi/
---

**Ruby on Rails posts:**
<ul>
  {% for post in site.categories.raspi %}
    <li>
      <a href="{{ post.url | prepend: site.github.url }}">{{ post.title }}</a>
      {{ post.excerpt }}
    </li>
  {% endfor %}
</ul>
