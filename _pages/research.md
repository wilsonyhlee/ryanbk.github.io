---
layout: page
permalink: /research/
title: research
years: [2024, 2023, 2022, 2021, 2020]
wp_years: [2024]
nav: true
---

<h2>Working Papers</h2>


<div class="publications">

{% for x in page.wp_years %}
  <h2 class="year">{{x}}</h2>
  {% bibliography -f working_papers -q @*[year={{x}}]* %}
{% endfor %}

</div>

<h2>Published Articles</h2>

<div class="publications">

{% for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>


