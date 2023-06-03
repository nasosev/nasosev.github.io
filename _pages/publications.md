---
layout: page
permalink: /publications/
title: Publications
description: Publications in reversed chronological order.
years: [2023,2019,2015] # make this a range
nav: true
nav_order: 1
---
<!-- _pages/publications.md -->
<div class="publications">

{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f {{ site.scholar.bibliography }} -q @*[year={{y}}]* %}
{% endfor %}

</div>
