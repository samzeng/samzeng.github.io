---
layout: page
title: reading
permalink: /reading.html
---

{% for group in site.data.reading %}
## {{ group.name }}
{% for item in group.children %}
* [{{ item.author }} - {{ item.name }}]({{ item.url }})
{% endfor %}
{% endfor %}
