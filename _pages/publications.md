---
layout: page
permalink: /publications/
title: publications
description: Publications in reversed chronological order. 
years: [2023, 2022, 2021, 2020, 2019, 2018, 2017, 2016, 2015]
nav: true
nav_order: 1
---
<!-- _pages/publications.md -->
<div class="publications">
An up-to-date list is available on <a href='(https://scholar.google.com/citations?user=UqNe4lIAAAAJ&hl=en' target='_blank'>Google scholar</a> 
{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f {{ site.scholar.bibliography }} -q @*[year={{y}}]* %}
{% endfor %}

</div>
