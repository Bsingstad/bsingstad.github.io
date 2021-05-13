---
layout: page
permalink: /publication/
title: publication
order: 3
description: >
  Hope this list never ends😊
years: [2020, 2019, 2017]
nav: true
---

<div class="publications">

{% for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
