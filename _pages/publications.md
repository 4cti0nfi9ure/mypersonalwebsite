---
layout: page
permalink: /publications/
title: Publications
description: Publications by categories in reversed chronological order.
years: [2022,2021,2020,2019,2018,2017,2016,2015]
nav: true
nav_order: 2
---
<!-- _pages/publications.md -->
<div class="publications">

<h2 align="left">Journal and magazine articles</h2>

{% bibliography -f journals %}

<h2 align="left">Conference papers</h2>

{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

<h2 align="left">Preprints</h2>

{% bibliography -f preprints %}

<h2 align="left">Books</h2>

{% bibliography -f books %}

<h2 align="left">Book chapters</h2>

{% bibliography -f bookchapters %}

<h2 align="left">Data sets</h2>

{% bibliography -f datasets %}

</div>
