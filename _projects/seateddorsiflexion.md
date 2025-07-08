---
layout: page
title: "Motorized Stretching Device"
permalink: /projects/seateddorsiflexion/
---

## Device
<img src="/assets/images/projects/stretching.png" alt="Motorized Stretching Device" class="project-img">

## Collaborators
Nicholas A. Rubino, Dr. Aiko Thompson, Dr. Victor H. Duenas (PI)

### Related Publications

{% assign filtered_pubs = site.data.publications | where: "tag", "Seated Dorsiflexion" %}

{% for pub in filtered_pubs %}
  {% include pub_card.html item=pub %}
{% endfor %}

### Related Presentations

{% for pres in site.data.presentations %}
  {% if pres.tag contains "Seated Dorsiflexion" %}
    {% include pub_card.html item=pres %}
  {% endif %}
{% endfor %}
