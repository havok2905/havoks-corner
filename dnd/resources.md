---
layout: page
title: Resources
permalink: /d&d/resources/
parent: d&d
card_image_url: /assets/img/tiles/resources-tile.png
---

<ul>
  {% for page in site.pages %}
    {% if page.parent == 'd&d/resources' %}
      <li>
        <a class="page-link" href="{{ page.url | relative_url }}">
          {{ page.title }}
        </a>
      </li>
    {% endif %}
  {% endfor %}
</ul>
