---
layout: page
title: Creatures
permalink: /d&d/creatures/
parent: d&d
card_image_url: /assets/img/tiles/creatures-tile.png
---

{% for page in site.pages %}
{% if page.parent == 'd&d/creatures' %}
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
