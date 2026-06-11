---
title: "Teaching"
permalink: /teaching/
author_profile: true
---

{% assign teaching_items = site.teaching | sort: "date" | reverse %}
{% for post in teaching_items %}
  {% include archive-single.html %}
{% endfor %}
