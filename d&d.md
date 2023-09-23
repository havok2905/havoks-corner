---
layout: page
title: D&D
permalink: /d&d/
---

<ul class="card-list">
  {% for page in site.pages %}
    {% if page.parent == 'd&d' %}
      <li class="card">
        <a class="page-link" href="{{ site.baseurl }}{{ page.url }}">
          <img src="{{page.card_image_url}}">
          <span>
            {{ page.title }}
          </span>
        </a>
      </li>
    {% endif %}
  {% endfor %}
</ul>