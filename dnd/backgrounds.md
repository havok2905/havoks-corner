---
layout: page
title: Backgrounds
permalink: /d&d/backgrounds/
parent: d&d
card_image_url: /assets/img/tiles/backgrounds-tile.png
---

{% for page in site.pages %}
{% if page.parent == 'd&d/backgrounds' %}
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
