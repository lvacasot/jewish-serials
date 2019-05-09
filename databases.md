---
layout: page
title: Raw Data
permalink: /database/
---

{{ site.data.periodicals }}

{% for periodical in site.data.periodicals %}
    {{periodical.name}}, {{periodical.publication_date}} - {{periodical.end_date}}, {{periodical.publication_type}}, {{periodical.city}}
{% endfor %}