---
layout: page
title: "Motorized Bicycle"
permalink: /projects/motorizedbicycle/
---

## Device
<img src="/assets/images/projects/bicycle.png" alt="Motorized Bicycle" class="project-img">

## Collaborators
Nicholas A. Rubino, Dr. Jonathan Casas, Dr. Cheng-Hao Chang, Dr. Steven Brose, Dr. Victor H. Duenas (PI)

### Related Publications

{% assign filtered_pubs = site.data.publications | where: "tag", "bicycle" %}

{% for pub in filtered_pubs %}
  {% include pub_card.html item=pub %}
{% endfor %}

### Related Presentations

{% for pres in site.data.presentations %}
  {% if pres.tag contains "bicycle" %}
    {% include pub_card.html item=pres %}
  {% endif %}
{% endfor %}
