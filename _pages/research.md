---
layout: page
permalink: /research/
title: Research
description: 
years_wp: [2025,2024]
years_progress: [2025]
years_pup: [2024]
nav: true
---
***
<div class="publications">
<h1 class="year">Working Papers</h1>
{% for y in page.years_wp %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}},topic=wp]* %}
{% endfor %}
</div>
***
<div class="publications">
<h1 class="year">Publications</h1>
{% for y in page.years_pup %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}},topic=pup]* %}
{% endfor %}
</div>
***
<div class="publications">
<h1 class="year">Work in Progress</h1>
{% for y in page.years_progress %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}},topic=wip]* %}
{% endfor %}
</div>
***



