---
layout: page
permalink: /publications/
title: Publications
description: Full publications on <a href=https://scholar.google.co.kr/citations?user=WSG4VC0AAAAJ=en  style=color:#389AC4>Google Scholar.</a><br> Asterik(*) means equal contribution.
years: [2024, 2023, 2022, 2021, 2019]
nav: true
nav_order: 3
---
<!-- _pages/publications.md -->
<div class="publications">

{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
