---
layout: page
permalink: /research/
title: research
years: [2024, 2023, 2022, 2021, 2020]
nav: true
---

<div class="publications">

{% for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>


<!-- <div class="publications">

{% for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f working_papers -q @*[year={{y}}]* %}
{% endfor %}

</div> -->
