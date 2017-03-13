---
layout: page
title: Swift
permalink: /swift/
---

**Swift posts:**
<ul>
  {% for post in site.categories.swift %}
    <li>
      <a href="{{ post.url | prepend: site.github.url }}">{{ post.title }}</a>
      {{ post.excerpt }}
    </li>
  {% endfor %}
</ul>
