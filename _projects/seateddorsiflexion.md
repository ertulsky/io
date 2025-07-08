---
layout: page
title: "Motorized Stretching Device"
permalink: /projects/seateddorsiflexion/
---

## Device

## Collaborators
Nicholas A. Rubino, Dr. Aiko Thompson, Dr. Victor H. Duenas (PI)

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

## Related Presentations

{% for pres in site.data.presentations %}
  {% if pres.tag contains "Seated Dorsiflexion" %}
    <div class="pub-entry">
      <a href="{{ pres.link }}" target="_blank">
        <img src="{{ pres.img }}" alt="{{ pres.title }}" class="pub-thumb">
      </a>
      <div class="pub-details">
        <a href="{{ pres.link }}" class="pub-title" target="_blank">{{ pres.title }}</a>
        <div class="pub-meta">{{ pres.venue }} (<strong>{{ pres.year }}</strong>)</div>
        <div class="pub-authors">{{ pres.authors }}</div>
        <div class="pub-year-inst">
          {% for t in pres.tag %}
            <a href="/tags/{{ t | slugify }}">{{ t }}</a>{% unless forloop.last %}, {% endunless %}
          {% endfor %}
        </div>
      </div>
    </div>
  {% endif %}
{% endfor %}
