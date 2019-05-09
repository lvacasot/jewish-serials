---
layout: page
title: Bolivia
permalink: /Bolivia/
---
<ul>
    {% for serial in site.data.Bolivia-English %}
        
        <li>
            | {{serial.Original}} | {{serial.Transliteration}} | {{serial.Title_in_Spanish}} | {{serial.Editor_Director}} | {{serial.Language}} | {{serial.Country}} | {{serial.Place_of_Edition}} | {{serial.Address}} | {{serial.Editor}} | {{serial.Type_of_Publication}} | {{serial.Start_Date}} - {{serial.End_Date}} | {{serial.Frequency}} | {{serial.Clasification}} | {{serial.Notes}} | {{serial.Repository}} |
            <br><br>
        </li>   
        
    {% endfor %}

</ul>