---
layout: default
title: Travel
permalink: /trave/
---

{% for post in site.posts %}
 {% if post.tags contains "travel" %}
  {% include excerpt.html %}
 {% endif %}
{% endfor %}

{% if site.tags.travel == null %}
  <p>There aren't any posts about travel yet :(</p>
{% endif %}
