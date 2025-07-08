---
layout: page
title: "Ankle Foot Orthosis"
permalink: /projects/anklefootorthosis/
---

## Device
<img src="/assets/images/projects/ankledevice_6-27-2024.png" alt="Motorized Stretching Device" class="project-img">

## Collaborators
Nicholas A. Rubino, Jade Carter, Dr. Aiko Thompson, Dr. Victor H. Duenas (PI)

### Related Publications

{% assign filtered_pubs = site.data.publications | where: "tag", "Ankle Foot Orthosis" %}

{% for pub in filtered_pubs %}
  {% include pub_card.html item=pub %}
{% endfor %}

### Related Presentations

{% for pres in site.data.presentations %}
  {% if pres.tag contains "Ankle Foot Orthosis" %}
    {% include pub_card.html item=pres %}
  {% endif %}
{% endfor %}

### Ongoing Projects
- Support vector machine, an ML technique, to characterize the gait phase.
