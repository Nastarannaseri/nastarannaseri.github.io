---
layout: page
permalink: /publications/
title: Publications
description: Below you will find a list of my recent publications in academic journals, in conference proceedings.
years: [2017, 2019, 2021, 2022]
nav: true
nav_order: 1
---
<!-- _pages/publications.md -->
<div class="publications">

{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
