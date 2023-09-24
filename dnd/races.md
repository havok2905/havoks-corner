---
layout: page
title: Races
permalink: /d&d/races/
parent: d&d
card_image_url: /assets/img/tiles/races-tile.png
---

<ul>
  {% for page in site.pages %}
    {% if page.parent == 'd&d/races' %}
      <li>
        <a class="page-link" href="{{ page.url | relative_url }}">
          {{ page.title }}
        </a>
      </li>
    {% endif %}
  {% endfor %}
</ul>
