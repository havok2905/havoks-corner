---
layout: page
title: Resources
permalink: /d&d/resources/
parent: d&d
card_image_url: /assets/img/tiles/resources-tile.png
---

{% for page in site.pages %}
{% if page.parent == 'd&d/resources' %}
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
