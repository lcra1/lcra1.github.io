---
title: testpage
description: this is test page
layout: default
---

## pagelist
{% capture pagelist%}{{ site.html_pages | sort }}{% endcapture%}
{% for p in page.pagelist %}
- [{{ p.title }}]({{ site.github.url }}{{ p.url }})
{% endfor %}
