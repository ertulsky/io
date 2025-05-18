---
layout: page
title: "Publications"
permalink: /Publications/
main_nav: true
---

## Conference Publications

{% for pub in site.data.publications %}
<div class="pub-entry">
  <a href="{{ pub.link }}" target="_blank">
    <img src="{{ pub.img }}" alt="Publication Image" class="pub-thumb">
  </a>
  <div class="pub-details">
    <a href="{{ pub.link }}" class="pub-title" target="_blank">{{ pub.title }}</a>
    <div class="pub-meta">{{ pub.venue }}</div>
    <div class="pub-authors">{{ pub.authors }}</div>
  </div>
</div>
{% endfor %}

## Presentations

{% for pres in site.data.presentations %}
<div class="pub-entry">
  <a href="{{ pres.link }}" target="_blank">
    <img src="{{ pres.img }}" alt="Presentation Image" class="pub-thumb">
  </a>
  <div class="pub-details">
    <a href="{{ pres.link }}" class="pub-title" target="_blank">{{ pres.title }}</a>
    <div class="pub-meta">{{ pres.venue }}</div>
    <div class="pub-authors">{{ pres.authors }}</div>
  </div>
</div>
{% endfor %}

