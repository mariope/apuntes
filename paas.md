---
layout: page
title: PaaS
permalink: /paas/
---

**PaaS posts:**
<ul>
  {% for post in site.categories.paas %}
    <li>
      <a href="{{ post.url | prepend: site.github.url }}">{{ post.title }}</a>
      {{ post.excerpt }}
    </li>
  {% endfor %}
</ul>
