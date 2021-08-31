---
layout: default
title: Discussion
parent: Risk
grand_parent: Projects
nav_order: 2
external_css:
- https://cdnjs.cloudflare.com/ajax/libs/font-awesome/4.7.0/css/font-awesome.min
custom_css:
- tooltips
external_js:
- https://ajax.googleapis.com/ajax/libs/jquery/3.5.1/jquery.min
custom_js:
- latex
---

# Discussion
{: .no_toc }

<br>

## Table of contents
{: .no_toc .text-delta }

1. TOC
{:toc}

---

### Of Model

It has been noted in a number of research papers [ref. identifiers] ...

<script id="roc"
  url="https://raw.githubusercontent.com/exhypotheses/risk/develop/warehouse/evaluations/model/metrics.json"
  src="{{ site.baseurl }}/assets/js/risk/roc.js" type="text/javascript"></script>
<div id="container0002" style="height: 350px; width: 300px; margin: 0 auto"></div>

<br>
<br>

### At Threshold

The model metrics at the optimal threshold are illustrated by the polygon graph.  It ...

<script id="scores"
  url="https://raw.githubusercontent.com/exhypotheses/risk/develop/warehouse/evaluations/model/scores.json"
  src="{{ site.baseurl }}/assets/js/risk/scores.js" type="text/javascript"></script>
<div id="container0001" style="height: 400px; width: 330px; margin: 0 auto"></div>

<br>
<br>

### Of Disaggregates

The target variable, reasonable [risk], has 2 unique elements: 1 (reasonable), 0 (unreasonable).  The
performance of the model w.r.t. each element is outlined in the ...

<br>
<br>
<br>
<br>


<script src="https://code.highcharts.com/highcharts.js"></script>
<script src="https://code.highcharts.com/highcharts-more.js"></script>
<script src="https://code.highcharts.com/modules/exporting.js"></script>
<script src="https://code.highcharts.com/modules/export-data.js"></script>
<script src="https://code.highcharts.com/modules/accessibility.js"></script>
<script src="https://code.highcharts.com/modules/annotations.js"></script>