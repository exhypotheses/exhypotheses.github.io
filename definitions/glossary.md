---
layout: default
title: Glossary
parent: Definitions
nav_order: 1
external_css:
- https://cdnjs.cloudflare.com/ajax/libs/font-awesome/4.7.0/css/font-awesome.min
custom_css:
- tooltips
- lists
external_js:
- https://ajax.googleapis.com/ajax/libs/jquery/3.5.1/jquery.min
custom_js:
- latex
---

# Glossary
{: .no_toc }

<br>

## Table of contents
{: .no_toc .text-delta }

1. TOC
{:toc}

---

## Glossary

Later, add annotations w.r.t.

<div style="margin-left: 60px">
  <ul>
    <li>$\small tpr$ = $\large \frac{tp}{tp + fn}$ = $\small 1 - fnr$</li>
    <li>$\small fnr$ = $\large \frac{fn}{tp + fn}$ = $\small 1 - tpr$</li>
    <li>$\small fpr$ = $\large \frac{fp}{fp + tn}$ = $\small 1 - tnr$</li>
    <li>$\small tnr$ = $\large \frac{tn}{fp + tn}$ = $\small 1 - fpr$</li>
  </ul>
</div>

<br>

<table style="width: 65%;font-size: 65%;text-align: left;">
  <colgroup>
      <col style="width: 15%">
      <col style="width: 55%">
      <col style="width: 20%">
      <col style="width: 10%">
  </colgroup>
  {% for row in site.data.definitions.glossary %}
    {% if forloop.first %}
    <tr>
      {% for pair in row %}
        <th>{{ pair[0] }}</th>
      {% endfor %}
    </tr>
    {% endif %}

    {% tablerow pair in row %}
      {{ pair[1] }}
    {% endtablerow %}
  {% endfor %}
</table>

<br>
<br>
<br>
<br>
