---
permalink: /research/index.html
layout: page
title: research
order: 3
---

```
More coming soon...
```

<!--
{% for item in site.pages %}
  <h2>{{ item.title }}</h2>
  <p>{{ item.description }}</p>
  <p><a href="{{ item.url }}">{{ item.title }}</a></p>
{% endfor %}
-->

{% assign sorted_pages = site.research | sort:"order" %}
{% for item in sorted_pages %}
 <!-- <h2>{{ item.title }}</h2>-->
  <!--<p>{{ item.description }}</p>-->
  <h2><a href="{{ item.url }}">{{ item.title }}</a></h2>
  <p>{{ item.description }}</p>
{% endfor %}

