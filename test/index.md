---
title: testpage
description: this is test page
layout: default
pagelist:
{% for p in site.html_pages %}
  - url: {{ p.url }}
    title: {{ p.title }}
{% endfor %}
---

## pagelist
{% assign sorted_pagelist = pagelist | sort %}
{% for p in page.sorted_pagelist %}
{{ p.url | replace: "*/", "  " | remove: "*" }}- [{{ p.title }}]({{ site.github.url }}{{ p.url }})
{% endfor %}
