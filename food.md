---
layout: default
title: Food
permalink: /food/
---

{% for post in site.posts %}
 {% if post.tags contains "food" %}
  {% include excerpt.html %}
 {% endif %}
{% endfor %}

{% if site.tags.food == null %}
  <p>There aren't any posts about food yet :(</p>
{% endif %}
