---
layout: page
title: Backgrounds
permalink: /d&d/backgrounds/
parent: d&d
card_image_url: /assets/img/tiles/backgrounds-tile.png
---

<ul>
  {% for page in site.pages %}
    {% if page.parent == 'd&d/backgrounds' %}
      <li>
        <a class="page-link" href="{{ page.url | relative_url }}">
          {{ page.title }}
        </a>
      </li>
    {% endif %}
  {% endfor %}
</ul>
