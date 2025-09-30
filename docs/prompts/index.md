---
title: Prompts
layout: default
---

# Prompts publicados

<ul>
{% assign pages = site.pages | where_exp: "p", "p.path contains 'prompts/'" %}
{% for p in pages %}
  {% if p.name != 'index.md' %}
  <li><a href="{{ p.url }}">{{ p.hu | default: p.title | default: p.name }}</a></li>
  {% endif %}
{% endfor %}
</ul>
