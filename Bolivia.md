---
layout: page
title: Bolivia
permalink: /Bolivia/
---
{% assign mydata=site.data.Bolivia%}

<table id="boliviadata">
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
    var table = new Tabulator("#boliviadata", {});
</script>





<ul>
    {% for serial in site.data.Bolivia-English %}
        
        <li>
            | {{serial.Original}} | {{serial.Transliteration}} | {{serial.Title_in_Spanish}} | {{serial.Editor_Director}} | {{serial.Language}} | {{serial.Country}} | {{serial.Place_of_Edition}} | {{serial.Address}} | {{serial.Editor}} | {{serial.Type_of_Publication}} | {{serial.Start_Date}} - {{serial.End_Date}} | {{serial.Frequency}} | {{serial.Clasification}} | {{serial.Notes}} | {{serial.Repository}} |
            <br><br>
        </li>   
        
    {% endfor %}

</ul>