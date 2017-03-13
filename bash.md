---
layout: page
title: Bash
permalink: /bash/
---

**Bash posts:**
<ul>
  {% for post in site.categories.bash %}
    <li>
      <a href="{{ post.url | prepend: site.github.url }}">{{ post.title }}</a>
      {{ post.excerpt }}
    </li>
  {% endfor %}
</ul>
