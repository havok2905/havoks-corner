---
layout: page
title: Magic Items
permalink: /d&d/magic-items
parent: d&d
card_image_url: /assets/img/tiles/magic-items-tile.png
---

<ul>
  {% for page in site.pages %}
    {% if page.parent == 'd&d/magic-items' %}
      <li>
        <a class="page-link" href="{{ site.baseurl }}{{ page.url }}">
          {{ page.title }}
        </a>
      </li>
    {% endif %}
  {% endfor %}
</ul>
