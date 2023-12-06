---
layout: page
title: Arkisto
permalink: /arkisto/
---
<h3>Fantasiametallipäiväkirjat</h3>
{% for category in site.categories %}{% if category[0] == 'fantasiametallipaivakirjat' %}
<ul>
    {% for post in category[1] %}
    <li><a href="{{ post.url }}">{{ post.title }}</a></li>
    {% endfor %}
</ul>
{% endif %}{% endfor %}
