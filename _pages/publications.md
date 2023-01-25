---
layout: page
permalink: /publications/
title: publications
nav: true
years: [2023]
# description: Please see google scholar for more update 
nav_order: 1
---
<!-- _pages/publications.md -->
<div class="publications">

{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
