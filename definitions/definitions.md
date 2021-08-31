---
layout: default
title: Definitions
nav_order: 3
has_children: true
permalink: /definitions
external_css:
- https://cdnjs.cloudflare.com/ajax/libs/font-awesome/4.7.0/css/font-awesome.min
custom_css:
- tooltips
external_js:
- https://ajax.googleapis.com/ajax/libs/jquery/3.5.1/jquery.min
custom_js:
- latex
---

# Definitions
{: .fs-9 }

Definitions of terms
{: .fs-6 .fw-300 }

<br>

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
