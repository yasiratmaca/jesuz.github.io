---
title: Categories
layout: page
permalink: /categories
---

{{site.categories}}

{% for cat in site.categories %}
<h3>{{cat[0] | capitalize}}</h3>
{% endfor %}