---
layout: page
title: Brasil
permalink: /Brasil/
---


{% assign mydata=site.data.Brasil %}

<table id="brasildata">
    <caption>Brasilian Serials</caption>
    <thead>
    {% for column in mydata[0] %}
        <th>{{ column[0] }}</th>
    {% endfor %}
    </thead>
    <tbody>
    {% for row in mydata %}
        <tr>
        {% for cell in row %}
            <td>{{ cell[1] }}</td>
        {% endfor %}
        </tr>
    {% endfor %}
    </tbody>
</table>

<script>
    var table = new Tabulator("#brasildata", {
        layout:"fitData",
        tooltips:true,
    });
</script>

