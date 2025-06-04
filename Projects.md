---
layout: page
title: "Projects"
permalink: /Projects/
main_nav: true
---

<style>
.project-section {
  margin-bottom: 40px;
}
.project-sub {
  display: flex;
  align-items: flex-start;  /* aligns image to the top of the text block */
  margin-bottom: 25px;
}

.project-img {
  width: 50px;
  height: auto;
  margin-right: 10px;
  border-radius: 6px;
  object-fit: contain;
  flex-shrink: 0;
  align-self: flex-start;   /* ensures the image aligns to top vertically */
}



.project-details {
  flex: 2;
}
.project-tag {
  font-size: 1.2em;
  font-weight: normal;
  color: #005f83;
  text-decoration: none;
}
.project-tag:hover {
  text-decoration: underline;
}
.project-meta {
  font-size: 0.85em;
  color: #555;
  margin-top: 4px;
}
</style>

## Rehabilitation Robotics

#### [Gait Phase Detection](/tags/gait-phase-detection)
<div class="project-sub">
  <img src="/assets/images/projects/MRI.jpg" alt="Gait Phase Detection" class="project-img">
  <div class="project-details">
    <div class="project-meta">Tags: {% assign tags = 'Kessler Foundation, Reinforcement Learning' | split: ', ' %}{% for tag in tags %}<a href="/tags/{{ tag | slugify }}">{{ tag }}</a>{% unless forloop.last %}, {% endunless %}{% endfor %}<br>Language: {% assign langs = 'Matlab' | split: ', ' %}{% for lang in langs %}<a href="/tags/{{ lang | slugify }}">{{ lang }}</a>{% unless forloop.last %}, {% endunless %}{% endfor %}</div>
  </div>
</div>

#### [Motorized Stretching Device](/tags/motorized-stretching-device)
<div class="project-sub">
  <img src="/assets/images/projects/stretching.png" alt="Motorized Stretching Device" class="project-img">
  <div class="project-details">
    <div class="project-meta"><em>Award: 1 conference paper</em></div>
Tags: {% assign tags = 'BSC Lab at SU, Model-Based Control' | split: ', ' %}{% for tag in tags %}<a href="/tags/{{ tag | slugify }}">{{ tag }}</a>{% unless forloop.last %}, {% endunless %}{% endfor %}<br>Language: {% assign langs = 'Matlab' | split: ', ' %}{% for lang in langs %}<a href="/tags/{{ lang | slugify }}">{{ lang }}</a>{% unless forloop.last %}, {% endunless %}{% endfor %}</div>
  </div>

#### [Ankle Foot Orthosis](/tags/ankle-foot-orthosis)
<div class="project-sub">
  <img src="/assets/images/projects/ankledevice_6-27-2024.png" alt="Ankle Foot Orthosis" class="project-img">
  <div class="project-details">
    <div class="project-meta"><em>Award: 1 conference paper, 1 thesis</em></div>
Tags: {% assign tags = 'BSC Lab at SU, Model-Based Control' | split: ', ' %}{% for tag in tags %}<a href="/tags/{{ tag | slugify }}">{{ tag }}</a>{% unless forloop.last %}, {% endunless %}{% endfor %}<br>Language: {% assign langs = 'Matlab' | split: ', ' %}{% for lang in langs %}<a href="/tags/{{ lang | slugify }}">{{ lang }}</a>{% unless forloop.last %}, {% endunless %}{% endfor %}</div>
  </div>

#### [Bicycle](/tags/bicycle)
<div class="project-sub">
  <img src="/assets/images/projects/bicycle.png" alt="Bicycle Project" class="project-img">
  <div class="project-details">
    <div class="project-meta"><em>Award: 1 conference paper, 1 thesis</em></div>
Tags: {% assign tags = 'BSC Lab at SU, Model-Based Control' | split: ', ' %}{% for tag in tags %}<a href="/tags/{{ tag | slugify }}">{{ tag }}</a>{% unless forloop.last %}, {% endunless %}{% endfor %}<br>Language: {% assign langs = 'Matlab' | split: ', ' %}{% for lang in langs %}<a href="/tags/{{ lang | slugify }}">{{ lang }}</a>{% unless forloop.last %}, {% endunless %}{% endfor %}</div>
  </div>

## Personal Projects

#### [Computer Vision Two-Link Robot Manipulator](/tags/robot-vision)
<div class="project-sub">
  <img src="/assets/images/projects/robot-vision.jpg" alt="Robot Vision" class="project-img">
  <div class="project-details">
    <div class="project-meta">Tags: {% assign tags = 'Personal Project, Reinforcement Learning' | split: ', ' %}{% for tag in tags %}<a href="/tags/{{ tag | slugify }}">{{ tag }}</a>{% unless forloop.last %}, {% endunless %}{% endfor %}<br>Language: {% assign langs = 'C++, Python' | split: ', ' %}{% for lang in langs %}<a href="/tags/{{ lang | slugify }}">{{ lang }}</a>{% unless forloop.last %}, {% endunless %}{% endfor %}</div>
  </div>
</div>

#### [Convex Optimization LP for Fantasy Football/Baseball](/tags/convex-optimization)
<div class="project-sub">
  <img src="/assets/images/projects/fantasy.png" alt="Fantasy Optimization" class="project-img">
  <div class="project-details">
    <div class="project-meta">Tags: {% assign tags = 'Personal Project' | split: ', ' %}{% for tag in tags %}<a href="/tags/{{ tag | slugify }}">{{ tag }}</a>{% unless forloop.last %}, {% endunless %}{% endfor %}<br>Language: {% assign langs = 'Python' | split: ', ' %}{% for lang in langs %}<a href="/tags/{{ lang | slugify }}">{{ lang }}</a>{% unless forloop.last %}, {% endunless %}{% endfor %}</div>
  </div>
</div>

#### [Motorized Window Blinds](/tags/window-blinds)
<div class="project-sub">
  <img src="/assets/images/projects/blinds.png" alt="Window Blinds" class="project-img">
  <div class="project-details">
    <div class="project-meta">Tags: {% assign tags = 'Personal Project' | split: ', ' %}{% for tag in tags %}<a href="/tags/{{ tag | slugify }}">{{ tag }}</a>{% unless forloop.last %}, {% endunless %}{% endfor %}<br>Language: {% assign langs = 'Arduino IDE' | split: ', ' %}{% for lang in langs %}<a href="/tags/{{ lang | slugify }}">{{ lang }}</a>{% unless forloop.last %}, {% endunless %}{% endfor %}</div>
  </div>
</div>

#### [Concussion Sensor](/tags/concussion-sensor)
<div class="project-sub">
  <img src="/assets/images/projects/footballhelmet.jpg" alt="Concussion Sensor" class="project-img">
  <div class="project-details">
    <div class="project-meta"><em>Award: Maxwell Citizens Finalist</em></div>
Tags: {% assign tags = 'Personal Project' | split: ', ' %}{% for tag in tags %}<a href="/tags/{{ tag | slugify }}">{{ tag }}</a>{% unless forloop.last %}, {% endunless %}{% endfor %}<br>Language: {% assign langs = 'Arduino IDE' | split: ', ' %}{% for lang in langs %}<a href="/tags/{{ lang | slugify }}">{{ lang }}</a>{% unless forloop.last %}, {% endunless %}{% endfor %}</div>
  </div>
