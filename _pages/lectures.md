---
layout: page
permalink: /lectures/
title: lectures
description:
years: [Day 0, Day 1, Day 2, Day 3]
nav: true
nav_order: 2
---
A list of publications in journals and conference proceedings, by year of publication for published articles, and year of submission for preprints. A list of works is also available on [Google Scholar](https://scholar.google.com/citations?user=mghzVekAAAAJ&hl=en).

*Copyright note.* This material is presented here to ensure timely dissemination of scholarly and technical work. Copyright and all rights therein are retained by authors or by the copyright holders. All persons accessing this information are expected to adhere to the terms and constraints invoked by each case’s copyright. Unless permitted by the license, these works may not be copied or re-posted without explicit permission.

<!-- _pages/publications.md -->
<div class="publications">

{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f lectures -q @*[year={{y}}]* %}
{% endfor %}

</div>