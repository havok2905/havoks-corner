---
layout: page
title: Creatures
permalink: /d&d/creatures
parent: d&d
card_image_url: /assets/img/tiles/creatures-tile.png
---

<ul>
  {% for page in site.pages %}
    {% if page.parent == 'd&d/creatures' %}
      <li>
        <a class="page-link" href="{{ page.url | relative_url }}">
          {{ page.title }}
        </a>
      </li>
    {% endif %}
  {% endfor %}
</ul>
