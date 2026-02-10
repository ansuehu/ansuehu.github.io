---
layout: default
title: Nire Proiektuak
---

<ul>
{% for file in site.static_files %}
  {% if file.extname == ".html" %}
    <li><a href="{{ file.path }}">{{ file.basename }}</a></li>
  {% endif %}
{% endfor %}
</ul>
