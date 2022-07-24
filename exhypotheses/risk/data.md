---
layout: default
title: Data
parent: Risk
grand_parent: Cases
nav_order: 2
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


## Definitions

The variables of the loan risk data set; none of the fields is nullable.

<br>

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

<br>
<br>

<br>
<br>

<br>
<br>
