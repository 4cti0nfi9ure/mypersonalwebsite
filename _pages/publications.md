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

<h2 align="left">Keynotes and invited talks</h2>

{% bibliography -f talks %}

<h2 align="left">Panels</h2>

{% bibliography -f panels %}

<h2 align="left">Programm committee memberships</h2>

<ul>
<li><a href="https://iwosemc.eu/">IWoSeMC-22</a>@<a href="https://fcrlab.unime.it/ccgrid22/">CCGrid 2022</a> 3<sup>rd</sup> International Workshop on Secure Mobile Cloud Computing (colocated The 22<sup>nd</sup> IEEE/ACM International Symposium on Cluster, Cloud and Internet Computing); May 16-May 19, 2022; Taormina (Messina), Italy.</li>

<li><a href="https://2021.ares-conference.eu/workshops-eu-symposium/ng-soc-2021/index.html">NG-SCO 2021</a>@<a href="https://2021.ares-conference.eu/">ARES 2021</a> 3<sup>rd</sup> International Workshop on Next Generation Security Operations Centers (NG-SOC 2021)  (colocated with The 16<sup>th</sup> International Conference on Availability, Reliability and Security); August 17-August 20, 2021; virtual conference.</li>

<li><a href="https://2021.iwosemc.eu/">IWoSeMC-21</a>@<a href="http://cloudbus.org/ccgrid2021/">CCGrid 2021</a> 2<sup>nd</sup> International Workshop on Secure Mobile Cloud Computing (colocated with The 21<sup>st</sup> IEEE/ACM International Symposium on Cluster, Cloud and Internet Computing); May 10-May 13, 2021; Melbourne, Victoria, Australia (virtual conference).</li>

<li><a href="https://www.astrid-project.eu/secsoft/tpc.html">SecSoft</a>@<a href="https://netsoft2020.ieee-netsoft.org/">NetSoft 2020</a>; 2<sup>nd</sup> International Workshop on Cyber-Security Threats, Trust and Privacy Management in Software-defined and Virtualized Infrastructures (colocated with The 6<sup>th</sup> IEEE International Conference on Network Softwarization); June 29-July 3, 2020; Ghent, Belgium (virtual conference).</li>
</ul>

<h2 align="left">Patents</h2>

{% bibliography -f patents %}

</div>
