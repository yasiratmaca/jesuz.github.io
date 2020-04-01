---
title: Categories
layout: default
permalink: /categories
---



{%- for cat in site.categories -%}
<h3>{{cat[0] | capitalize}}</h3>
<ul>
    {%- for post in cat[1] -%}

    <li>
    <a href="{{post.url}}">{{post.title}}</a>
    </li>
    {%- endfor -%}
</ul>

{% endfor %}


