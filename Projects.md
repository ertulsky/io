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
  align-items: flex-start;
  margin-bottom: 25px;
}
.project-img {
  width: 70px;
  height: auto;
  margin-right: 10px;
  border-radius: 6px;
  object-fit: cover;
}
.project-details {
  flex: 1;
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

### [Camera Gait Analysis](/tags/Camera-Gait-Analysis)
<div class="project-sub">
  <img src="/assets/images/projects/gait-phase.png" alt="Camera Gait Analysis" class="project-img">
  <div class="project-details">
    <div class="project-meta">Tags: {% assign tags = 'Kessler Foundation, Reinforcement Learning' | split: ', ' %}{% for tag in tags %}<a href="/tags/{{ tag | slugify }}">{{ tag }}</a>{% unless forloop.last %}, {% endunless %}{% endfor %}<br>Language: {% assign langs = 'Matlab' | split: ', ' %}{% for lang in langs %}<a href="/tags/{{ lang | slugify }}">{{ lang }}</a>{% unless forloop.last %}, {% endunless %}{% endfor %}</div>
  </div>
</div>

### [Motorized Stretching Device](/tags/motorized-stretching-device)
<div class="project-sub">
  <img src="/assets/images/projects/stretching.png" alt="Motorized Stretching Device" class="project-img">
  <div class="project-details">
    <a href="/tags/motorized-stretching-device" class="project-tag">Motorized Stretching Device</a>
    <div class="project-meta">Tags: {% assign tags = 'BSC Lab at SU, Model-Based Control' | split: ', ' %}{% for tag in tags %}<a href="/tags/{{ tag | slugify }}">{{ tag }}</a>{% unless forloop.last %}, {% endunless %}{% endfor %}<br>Language: {% assign langs = 'Matlab' | split: ', ' %}{% for lang in langs %}<a href="/tags/{{ lang | slugify }}">{{ lang }}</a>{% unless forloop.last %}, {% endunless %}{% endfor %}</div>
  </div>
</div>

### [Ankle Foot Orthosis](/tags/ankle-foot-orthosis)
<div class="project-sub">
  <img src="/assets/images/projects/ankle.png" alt="Ankle Foot Orthosis" class="project-img">
  <div class="project-details">
    <a href="/tags/ankle-foot-orthosis" class="project-tag">Ankle Foot Orthosis</a>
    <div class="project-meta">Tags: {% assign tags = 'BSC Lab at SU, Model-Based Control' | split: ', ' %}{% for tag in tags %}<a href="/tags/{{ tag | slugify }}">{{ tag }}</a>{% unless forloop.last %}, {% endunless %}{% endfor %}<br>Language: {% assign langs = 'Matlab' | split: ', ' %}{% for lang in langs %}<a href="/tags/{{ lang | slugify }}">{{ lang }}</a>{% unless forloop.last %}, {% endunless %}{% endfor %}</div>
  </div>
</div>

### [Bicycle](/tags/bicycle)
<div class="project-sub">
  <img src="/assets/images/projects/bicycle.png" alt="Bicycle Project" class="project-img">
  <div class="project-details">
    <a href="/tags/bicycle" class="project-tag">Bicycle</a>
    <div class="project-meta">Tags: {% assign tags = 'BSC Lab at SU, Model-Based Control' | split: ', ' %}{% for tag in tags %}<a href="/tags/{{ tag | slugify }}">{{ tag }}</a>{% unless forloop.last %}, {% endunless %}{% endfor %}<br>Language: {% assign langs = 'Matlab' | split: ', ' %}{% for lang in langs %}<a href="/tags/{{ lang | slugify }}">{{ lang }}</a>{% unless forloop.last %}, {% endunless %}{% endfor %}</div>
  </div>
</div>

## Personal Projects

### [Computer Vision Two-Link Robot Manipulator](/tags/robot-vision)
<div class="project-sub">
  <img src="/assets/images/projects/robot-vision.png" alt="Robot Vision" class="project-img">
  <div class="project-details">
    <a href="/tags/robot-vision" class="project-tag">Computer Vision Two-Link Robot Manipulator</a>
    <div class="project-meta">Tags: {% assign tags = 'Personal Project, Reinforcement Learning' | split: ', ' %}{% for tag in tags %}<a href="/tags/{{ tag | slugify }}">{{ tag }}</a>{% unless forloop.last %}, {% endunless %}{% endfor %}<br>Language: {% assign langs = 'C++, Python' | split: ', ' %}{% for lang in langs %}<a href="/tags/{{ lang | slugify }}">{{ lang }}</a>{% unless forloop.last %}, {% endunless %}{% endfor %}</div>
  </div>
</div>

### [Convex Optimization LP for Fantasy Football/Baseball](/tags/convex-optimization)
<div class="project-sub">
  <img src="/assets/images/projects/fantasy.png" alt="Fantasy Optimization" class="project-img">
  <div class="project-details">
    <a href="/tags/convex-optimization" class="project-tag">Convex Optimization LP for Fantasy Football/Baseball</a>
    <div class="project-meta">Tags: {% assign tags = 'Personal Project' | split: ', ' %}{% for tag in tags %}<a href="/tags/{{ tag | slugify }}">{{ tag }}</a>{% unless forloop.last %}, {% endunless %}{% endfor %}<br>Language: {% assign langs = 'Python' | split: ', ' %}{% for lang in langs %}<a href="/tags/{{ lang | slugify }}">{{ lang }}</a>{% unless forloop.last %}, {% endunless %}{% endfor %}</div>
  </div>
</div>

### [Motorized Window Blinds](/tags/window-blinds)
<div class="project-sub">
  <img src="/assets/images/projects/blinds.png" alt="Window Blinds" class="project-img">
  <div class="project-details">
    <a href="/tags/window-blinds" class="project-tag">Motorized Window Blinds</a>
    <div class="project-meta">Tags: {% assign tags = 'Personal Project' | split: ', ' %}{% for tag in tags %}<a href="/tags/{{ tag | slugify }}">{{ tag }}</a>{% unless forloop.last %}, {% endunless %}{% endfor %}<br>Language: {% assign langs = 'Arduino IDE' | split: ', ' %}{% for lang in langs %}<a href="/tags/{{ lang | slugify }}">{{ lang }}</a>{% unless forloop.last %}, {% endunless %}{% endfor %}</div>
  </div>
</div>

### [Concussion Sensor](/tags/concussion-sensor)
<div class="project-sub">
  <img src="/assets/images/projects/concussion.png" alt="Concussion Sensor" class="project-img">
  <div class="project-details">
    <a href="/tags/concussion-sensor" class="project-tag">Concussion Sensor</a>
    <div class="project-meta">Tags: {% assign tags = 'Personal Project' | split: ', ' %}{% for tag in tags %}<a href="/tags/{{ tag | slugify }}">{{ tag }}</a>{% unless forloop.last %}, {% endunless %}{% endfor %}<br>Language: {% assign langs = 'Arduino IDE' | split: ', ' %}{% for lang in langs %}<a href="/tags/{{ lang | slugify }}">{{ lang }}</a>{% unless forloop.last %}, {% endunless %}{% endfor %}</div>
  </div>
</div>
