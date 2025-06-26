---
title: Team
nav:
  order: 3
  tooltip: About our team
---

# {% include icon.html icon="fa-solid fa-users" %}Team

<span style="font-size: 20px; line-height: 1.4; display: block; margin-bottom: 10px;">


{% include section.html %}

## Principal Investigator
{% include list.html data="members" component="portrait" filter="role == 'pi'" %}

## Postdoctoral Fellows
{% include list.html data="members" component="portrait" filter="role == 'postdoc'" %}

## Graduate Students
{% include list.html data="members" component="portrait" filter="role == 'grad'" %}

## Research Assistants
{% include list.html data="members" component="portrait" filter="role == 'tech'" %}

{% include section.html background="images/background.jpg" dark=true %}

{% include section.html %}

{% capture content %}
{% include figure.html image="images/photo.jpg" %}
{% include figure.html image="images/photo.jpg" %}
{% include figure.html image="images/photo.jpg" %}
{% endcapture %}

{% include grid.html style="square" content=content %}
