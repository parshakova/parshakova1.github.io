---
layout: page
permalink: /publications/
title: publications
years: [2022, 2019, 2018, 2017, 2016]
nav: true
nav_order: 1
---

<div class="publications">

{% for y in page.years %}
  <div class="year">{{y}}</div>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}
</div>

