---
layout: page
title: Chile
permalink: /Chile/
---

{% assign mydata=site.data.Chile%}

<table id="chiledata">
    <caption>Chilean Serials</caption>
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
    var table = new Tabulator("#chiledata", {});
</script>