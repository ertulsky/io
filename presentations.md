---
layout: page
title: "Presentations"
permalink: /Thesis/
main_nav: true
---



<ul class="posts-list">
  {% for post in site.categories[cat] %}
    <li>
      <strong>
        <a href="{{ post.url | prepend: site.baseurl }}">{{ _posts/2024-05-20-Thesis.md }}</a>
      </strong>
    </li>
  {% endfor %}
  </ul>
  {% if forloop.last == false %}<hr>{% endif %}
{% endfor %}
<br>
