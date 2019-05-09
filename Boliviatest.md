---
layout: page
title: Bolivia Test
permalink: /Boliviat/
---

{% assign mydata=site.data.Bolivia-English %}

I can keep it in Spanish if I use the following code, but not sure how to display it properly yet other than the table format

{% for column in mydata[0] %}
    {{ column[0] }}
{% endfor %}

{% for row in mydata %}
    {% for cell in row %}
        {{ cell[1] }}
    {% endfor %}
{% endfor %}

<ul>
         {% for serial in site.data.Bolivia-English %}
            <li>
                {{serial}} <br><br>
            </li>
         {% endfor %}
</ul>