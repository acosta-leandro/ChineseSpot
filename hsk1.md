---
title: HSK-1
subtitle: Words from SK1
layout: "page"
icon: fa-book
order: 4
---

{% assign row = site.data.authors[0] %}
{% for pair in row %}
  {{ pair | inspect }}
{% endfor %}

<table>
  {% for row in site.data.authors %}
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