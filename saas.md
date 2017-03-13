---
layout: page
title: SaaS
permalink: /saas/
---

**SaaS posts:**
<ul>
  {% for post in site.categories.saas %}
    <li>
      <a href="{{ post.url | prepend: site.github.url }}">{{ post.title }}</a>
      {{ post.excerpt }}
    </li>
  {% endfor %}
</ul>
