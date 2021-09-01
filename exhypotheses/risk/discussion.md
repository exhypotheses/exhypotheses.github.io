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

### Introduction

The loan risk model's curves

<br>

<table style="width: 55%; border: 0;">
    <colgroup>
        <col span="1" style="width: 40%;">
        <col span="1" style="width: 40%;">
    </colgroup>
    <tr>
        <td><script id="roc"
            url="https://raw.githubusercontent.com/exhypotheses/risk/develop/warehouse/evaluations/model/metrics.json"
            src="{{ site.baseurl }}/assets/js/risk/roc.js" type="text/javascript"></script>
            <div id="container0002" style="height: 350px; width: 300px; margin: 0 auto"></div></td>
        <td><script id="ptc"
            url="https://raw.githubusercontent.com/exhypotheses/risk/develop/warehouse/evaluations/model/metrics.json"
            src="{{ site.baseurl }}/assets/js/risk/ptc.js" type="text/javascript"></script>
            <div id="container0003" style="height: 350px; width: 300px; margin: 0 auto"></div></td>
    </tr>
</table>

<br>
<br>
<br>
<br>

The loan risk model's metrics

<br>

<table style="width: 55%; align-content: center;">
    <colgroup>
        <col span="1" style="text-align: center;">
    </colgroup>        
    <tr>
        <td><script id="scores"
            url="https://raw.githubusercontent.com/exhypotheses/risk/develop/warehouse/evaluations/model/scores.json"
            src="{{ site.baseurl }}/assets/js/risk/scores.js" type="text/javascript"></script>
            <div id="container0001" style="height: 350px; width: 300px; margin: 0 auto"></div></td>
    </tr>
</table>

<br>
<br>
<br>
<br>

The metrics at various thresholds; the optimal threshold is at the intersection of precision & sensitivity (true positive rate).

<br>

<table style="width: 55%;">
    <colgroup>
        <col span="1" style="width: 35%;">
        <col span="1" style="width: 35%;">
    </colgroup>
    <tr>
        <td><script id="metrics"
            url="https://raw.githubusercontent.com/exhypotheses/risk/develop/warehouse/evaluations/model/metrics.json"
            src="{{ site.baseurl }}/assets/js/risk/metrics.js" type="text/javascript"></script>
            <div id="container0004" style="height: 390px; width: 330px;  margin: 0 auto"></div></td>
        <td><script id="frequencies"
            url="https://raw.githubusercontent.com/exhypotheses/risk/develop/warehouse/evaluations/model/frequencies.json"
            src="{{ site.baseurl }}/assets/js/risk/frequencies.js" type="text/javascript"></script>
            <div id="container0005" style="height: 390px; width: 330px;  margin: 0 auto"></div></td>
    </tr>
</table>

<br>
<br>
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
