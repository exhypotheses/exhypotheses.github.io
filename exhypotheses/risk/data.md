---
layout: default
title: Data
parent: Risk
grand_parent: Projects
nav_order: 1
custom_js:
- latex
---

# Data
{: .no_toc }

<br>

## Table of contents
{: .no_toc .text-delta }

1. TOC
{:toc}

---


## Introduction
<br>
<div>
      <p>The $p_{value}$ of each categorical field & target hypotheses ... $\chi^{2}$</p>
</div>

<br>
<br>

## Metadata
<br>
This section focuses on the data source, licence, # of instances, etc

<br>
<br>

## Definitions
<br>
None of the fields is nullable.

<table style="width: 65%;font-size: 65%;text-align: left;">
  {% for row in site.data.exhypotheses.risk.definitions %}
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

## Sample

<br>
<br>
<br>
<br>
