---
layout: page
title: Creatures
permalink: /d&d/creatures/
parent: d&d
card_image_url: /assets/img/tiles/creatures-tile.png
---

{% for page in site.pages %}
{% if page.parent == 'd&d/creatures' %}
  <div class="havok-design-blog-card">
    <div class="havok-design-blog-card-content">
      <h2>
        <a href="{{ page.url | relative_url }}">
          {{ page.title }}
        </a>
      </h2>
    </div>
  </div>
{% endif %}
{% endfor %}
