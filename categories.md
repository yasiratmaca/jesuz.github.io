---
title: Categories
layout: default
permalink: /categories
---

{{site.categories}}

{% for cat in site.categories %}
<h3>{{cat[0] | capitalize}}</h3>
    {% for post in cat[1] %}
    <li><a href="{{post.url}}">{{post.title}}</a></li>
    {% endfor %}


{% endfor %}