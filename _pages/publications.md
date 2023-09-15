---
layout: page
permalink: /publications/
title: publications
nav: true
nav_order: 1
---
<!-- _pages/publications.md -->
<div class="publications">

{% capture publications_size -%}
  {% bibliography_count -f {{ site.scholar.bibliography }} %}
{%- endcapture %}
{% if publications_size != "0" -%}
  {% bibliography -f {{ site.scholar.bibliography }} %}
{%- else -%}
  <p>No publications so far...</p>
{%- endif %}

</div>
