---
layout: page
title: "Motorized Stretching Device"
permalink: /projects/seateddorsiflexion/
---

# Motorized Stretching Device

## Collaborators
Nicholas A. Rubino
Victor H. Duenas (PI)

## Publications

## Related Publications

{% assign filtered_pubs = site.data.publications | where: "tag", "Seated Dorsiflexions" %}

{% for pub in filtered_pubs %}
<div class="pub-entry">
  <a href="{{ pub.link }}" target="_blank">
    <img src="{{ pub.img }}" alt="Publication Image" class="pub-thumb">
  </a>
  <div class="pub-details">
    <a href="{{ pub.link }}" class="pub-title" target="_blank">{{ pub.title }}</a>
    <div class="pub-meta">{{ pub.venue }} (<strong>{{ pub.year }}</strong>)</div>
    <div class="pub-authors">{{ pub.authors }}</div>
    <div class="pub-year-inst"><a href="/tags/{{ pub.tag | slugify }}">{{ pub.tag }}</a></div>
  </div>
</div>
{% endfor %}
