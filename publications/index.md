---
title: Publications
nav:
  order: 2
  tooltip: Published works
---

# {% include icon.html icon="fa-solid fa-microscope" %}Research



{% include section.html %}

{% include search-box.html %}

{% include search-info.html %}

## Highlighted



{% assign featured = site.data.citations | where: "featured", true %}
{% for pub in featured %}
  {% include citation.html lookup=pub.id style="rich" %}
{% endfor %}


## All



{% include list.html data="citations" component="citation" style="rich" %}
