---
title: testpage
description: this is test page
layout: default
---

## pagelist
{% assign pagelist = site.html_pages | sort %}
{% for p in page.pagelist %}
- [{{ p.title }}]({{ site.github.url }}{{ p.url }})
{% endfor %}
