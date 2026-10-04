---
layout: page
title: Publications
permalink: /publications/
---
{%- assign by_year = site.data.publications | group_by: "year" | sort: "name" | reverse -%}
{%- for group in by_year %}
<h2 class="year">{{ group.name }}</h2>
<ul class="pubs">
  {%- for pub in group.items %}
  {% include publication.html pub=pub %}
  {%- endfor %}
</ul>
{%- endfor %}
