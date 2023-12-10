---
layout: page
title: Magic Items
permalink: /d&d/magic-items/
parent: d&d
card_image_url: /assets/img/tiles/magic-items-tile.png
---

{% for page in site.pages %}
{% if page.parent == 'd&d/magic-items' %}
  <div>
    <a class="havok-design-system-blog-card" href="{{ page.url | relative_url }}">
      <div class="havok-design-blog-card-content">
        <h3>
          {{ page.title }}
        </h3>
      </div>
    </a>
  </div>
{% endif %}
{% endfor %}
