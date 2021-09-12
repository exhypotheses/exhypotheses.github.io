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

<table style="width: 65%;font-size: 65%;text-align: left;">
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
