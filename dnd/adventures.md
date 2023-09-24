---
layout: page
title: Adventures
permalink: /d&d/adventures
parent: d&d
card_image_url: /assets/img/tiles/adventures-tile.png
---

<ul>
  {% for page in site.pages %}
    {% if page.parent == 'd&d/adventures' %}
      <li>
        <a class="page-link" href="{{ page.url | relative_url }}">
          {{ page.title }}
        </a>
      </li>
    {% endif %}
  {% endfor %}
</ul>
