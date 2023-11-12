---
layout: page
title: D&D
permalink: /d&d/
---

<ul class="havok-design-tile-grid">
  {% for page in site.pages %}
    {% if page.parent == 'd&d' %}
      <li class="havok-design-tile">
        <a href="{{ page.url | relative_url }}">
          <img src="{{page.card_image_url | relative_url}}">
          <span>
            {{ page.title }}
          </span>
        </a>
      </li>
    {% endif %}
  {% endfor %}
</ul>