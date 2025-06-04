---
layout: page
title: "Publications"
permalink: /Publications/
main_nav: true
---

<style>
.pub-entry {
  display: flex;
  align-items: flex-start;
  margin-bottom: 30px;
  border-bottom: 1px solid #ddd;
  padding-bottom: 15px;
}

.pub-thumb {
  width: 60px;
  height: auto;
  max-height: 100px;
  margin-right: 20px;
  border-radius: 4px;
  object-fit: contain;
}

.pub-details {
  flex: 1;
}

.pub-title {
  font-size: 1.2em;
  font-weight: bold;
  color: #005f83;
  text-decoration: none;
}

.pub-title:hover {
  text-decoration: underline;
}

.pub-meta {
  font-style: italic;
  margin-top: 5px;
}

.pub-authors {
  margin-top: 5px;
  color: #444;
}

.pub-year-inst {
  margin-top: 5px;
  font-size: 0.9em;
  color: #666;
}
</style>

## Journal Articles
<p><em>No journal articles available at this time.</em></p>

## Conference Publications

{% for pub in site.data.publications %}
<div class="pub-entry">
  <a href="{{ pub.link }}" target="_blank">
    <img src="{{ pub.img }}" alt="Publication Image" class="pub-thumb">
  </a>
  <div class="pub-details">
    <a href="{{ pub.link }}" class="pub-title" target="_blank">{{ pub.title }}</a>
    <div class="pub-meta">{{ pub.venue }} (<strong>{{ pub.year }}</strong>)</div>
    <div class="pub-authors">{{ pub.authors }}</div>
    <div class="pub-year-inst"><a href="/tags/bsc-lab-at-su">BSC Lab at SU</a></div>
  </div>
</div>
{% endfor %}

## Thesis

<div class="pub-entry">
  <a href="https://evantulsky.netlify.app/papers/awards/2024/05/20/thesis" target="_blank">
    <img src="/assets/publications/thesis2024.png" alt="Honors Thesis" class="pub-thumb">
  </a>
  <div class="pub-details">
    <a href="https://evantulsky.netlify.app/papers/awards/2024/05/20/thesis" class="pub-title" target="_blank">
      Targeting the Soleus and Quadriceps Muscles Using Powered Robotic Rehabilitation Devices and Neuromuscular Control
    </a>
    <div class="pub-meta">Honors Thesis (<strong>2024</strong>)</div>
    <div class="pub-authors">Evan Tulsky</div>
    <div class="pub-year-inst"><a href="/tags/bsc-lab-at-su">BSC Lab at SU</a></div>
  </div>
</div>

## Presentations

{% for pres in site.data.presentations %}
<div class="pub-entry">
  <a href="{{ pres.link }}" target="_blank">
    <img src="{{ pres.img }}" alt="Presentation Image" class="pub-thumb">
  </a>
  <div class="pub-details">
    <a href="{{ pres.link }}" class="pub-title" target="_blank">{{ pres.title }}</a>
    <div class="pub-meta">{{ pres.venue }} (<strong>{{ pres.year }}</strong>)</div>
    <div class="pub-authors">{{ pres.authors }}</div>
    {% if pres.tag %}
    <div class="pub-year-inst"><a href="/tags/{{ pres.tag | slugify }}">{{ pres.tag }}</a></div>
    {% endif %}
  </div>
</div>
{% endfor %}

