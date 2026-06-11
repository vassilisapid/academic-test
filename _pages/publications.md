---
title: "Research"
permalink: /research/
author_profile: true
---

## Publications and preprints

{% assign pubs = site.publications | sort: "date" | reverse %}
{% for post in pubs %}
  {% include archive-single.html %}
{% endfor %}
