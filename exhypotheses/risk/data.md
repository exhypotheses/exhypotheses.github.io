---
layout: default
title: Data
parent: Credit Risk
grand_parent: Projects
nav_order: 1
custom_js:
- latex
---

# Querying
{: .no_toc }

<br>

## Table of contents
{: .no_toc .text-delta }

1. TOC
{:toc}

---


## Introduction
A brief introduction to the data sheets sections herein.

<br>

## Metadata
This section focuses on the data source, licence, # of instances, etc

<br>

## Definitions

<table style="width: 65%;font-size: small;text-align: left;">
  {% for row in site.data.risk.definitions %}
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

## Sample
A preview
