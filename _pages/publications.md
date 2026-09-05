---
title: "Research"
permalink: /research/
layout: single
author_profile: true
---

<div class="numbered-research" markdown="1">

## Preprints

{% assign preprints = site.publications | where: "category", "preprint" | sort: "date" | reverse %}
<ol class="research-items">
{% for post in preprints %}
  <li>{{ post.citation }}{% if post.paperurl %} <a href="{{ post.paperurl }}">[link]</a>{% endif %}</li>
{% endfor %}
</ol>

## Publications

### Journal publications

{% assign journal_pubs = site.publications | where: "category", "journal" | sort: "date" | reverse %}
<ol class="research-items">
{% for post in journal_pubs %}
  <li>{{ post.citation }}{% if post.paperurl %} <a href="{{ post.paperurl }}">[link]</a>{% endif %}</li>
{% endfor %}
</ol>

### Conference publications

{% assign conference_pubs = site.publications | where: "category", "conference" | sort: "date" | reverse %}
<ol class="research-items">
{% for post in conference_pubs %}
  <li>{{ post.citation }}{% if post.paperurl %} <a href="{{ post.paperurl }}">[link]</a>{% endif %}</li>
{% endfor %}
</ol>

## Dissertations

{% assign dissertations = site.publications | where: "category", "dissertation" | sort: "date" | reverse %}
<ol class="research-items">
{% for post in dissertations %}
  <li>{{ post.citation }}{% if post.paperurl %} <a href="{{ post.paperurl }}">[link]</a>{% endif %}</li>
{% endfor %}
</ol>

</div>
