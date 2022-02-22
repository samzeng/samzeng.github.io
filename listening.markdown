---
layout: page
title: listening
permalink: /listening.html
---

{% for group in site.data.listening %}
## {{ group.name }}
{% for item in group.children %}
* {{ item.artist }} - [{{ item.name }}]({{ item.url }})
{% endfor %}
{% endfor %}
