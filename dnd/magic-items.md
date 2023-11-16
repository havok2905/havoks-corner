---
layout: page
title: Magic Items
permalink: /d&d/magic-items/
parent: d&d
card_image_url: /assets/img/tiles/magic-items-tile.png
---

{% for page in site.pages %}
{% if page.parent == 'd&d/magic-items' %}
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
