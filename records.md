---
layout: page
title: Records
permalink: /records/
---
<table>
  <thead>
    <tr>
    {% for header in site.data.example.keys %}
      <td>{{header}}</td>
    {% endfor %}
    </tr>
  </thead>
  <tbody>
    {% for row in site.data.example.content %}
    <tr>
    {% for column in row %}
      <td>{{column}}</td>
    {% endfor %}
    </tr>
    {% endfor %}
  </tbody>
</table>

<ul>
    {% for serial in site.data.Colombia-airtable %}
        <li>
            {{serial.Titulo_Original}}
        </li>
    {% endfor %}
</ul>

#{% for item in serial %}
#    {{ item[0] }}
#   {% endfor %}