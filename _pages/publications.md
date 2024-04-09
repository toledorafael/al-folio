---
layout: page
permalink: /publications/
title: publications
description: 
years: [2024, 2023, 2021, 2020,  2014]
nav: true
---

<div class="publications">

{% for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
