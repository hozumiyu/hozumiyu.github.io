---
layout: page
permalink: /publications/
title: Publications
description: Also see <a href='https://scholar.google.com/citations?user=HU0hEb4AAAAJ&hl=en'>Google Scholar</a>
years: [2024, 2023, 2022, 2021, 2020, preparation]
nav: true
nav_order: 2
---
<!-- _pages/publications.md -->
<div class="publications">

{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
