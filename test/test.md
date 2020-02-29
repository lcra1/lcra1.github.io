---
---

## pagelist
<ul>
  {% for page in site.html_pages %}
  <li>
    :<a href="{{site.github.url}}{{ page.url }}">{{ page.title | remove: "/*.html" }}</a>
  </li>
  
  {% endfor %}
</ul>
		{% if headerLevel < minHeader or headerLevel > maxHeader %}
			{% continue %}
