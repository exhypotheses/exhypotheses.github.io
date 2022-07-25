---
layout: default
title: Graphs
parent: Risk
grand_parent: Cases
nav_order: 1
external_css:
- https://cdnjs.cloudflare.com/ajax/libs/font-awesome/4.7.0/css/font-awesome.min
custom_css:
- tooltips
external_js:
- https://ajax.googleapis.com/ajax/libs/jquery/3.5.1/jquery.min
custom_js:
- latex
---

# A sample of graphs for a classification model evaluation
{: .no_toc }

<br>

## Table of contents
{: .no_toc .text-delta }

1. TOC
{:toc}

---

These graphs illustrate the evaluation metrics of a binary classification model.  The model is for a loan risk 
binary classification problem; good 1, bad 0.  The values assigned by the model, to a test data set, are not 
exactly 0 or 1.  Rather, they are values within the range $[0 \; 1]$.  This leads to the question, beyond what
point within the range is a value equivalent to one?  Herein the point, known as the threshold, is the point 
at which precision & sensitivity (true positive rate) curves intersect.

Note, the graphs apply to any binary classification problem.

<br>

### ROC & Precision/Sensitivity Curves

The receiver operating and precision/sensitivity curves.

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

### The Evaluation Metrics at the Threshold

The range of each metric is $[0 \; 1]$; $1$ is the optimal value in each case.  <b>The tooltips per dot are upcoming</b>.

<br>

<script id="scores"
  url="https://raw.githubusercontent.com/exhypotheses/risk/develop/warehouse/evaluations/model/scores.json"
  src="{{ site.baseurl }}/assets/js/risk/scores.js" type="text/javascript">
</script>
<div id="container0001" style="height: 350px; width: 300px; margin: 0 auto"></div>

<br>
<br>

### The Binary Classification Metrics Curves

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
