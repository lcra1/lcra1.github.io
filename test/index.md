---
title: testpage
description: this is test page
layout: default
---

## pagelist
<ul>
  {% for page in site.html_pages %}
  <li>
    <a href="{{site.github.url}}{{ page.url }}">{{ page.url | remove: "/*.html" }}</a>
  </li>
  
  {% endfor %}
</ul>
