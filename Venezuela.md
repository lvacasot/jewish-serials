---
layout: page
title: Venezuela
permalink: /Venezuela/
---

{% assign mydata=site.data.Venezuela %}

<table id="venezueladata">
    <caption>Table caption</caption>
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
    var table = new Tabulator("#venezueladata", {});
</script>