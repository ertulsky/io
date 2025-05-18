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
