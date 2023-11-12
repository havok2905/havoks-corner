---
layout: page
title: Blog
permalink: /blog/
---

{%- if site.posts.size > 0 -%}
  {%- for post in site.posts -%}
    <div class="havok-design-blog-card">
      <div class="havok-design-blog-card-content">
        {%- if post.tags.size > 0 -%}
          <ul>
            {%- for tag in post.tags -%}
              <li>{{ tag }}</li>
            {%- endfor -%}
          </ul>
        {%- endif -%}
        <h2>
          <a href="{{ post.url | relative_url }}">
            {{ post.title | escape }}
          </a>
        </h2>
        <p>
          {{ post.excerpt }}
        </p>
        <p class="havok-design-blog-card-date">
          {%- assign date_format = site.minima.date_format | default: "%b %-d, %Y" -%}
          {{ post.date | date: date_format }}
        </p>
      </div>
    </div>
  {%- endfor -%}
  <p>
    <a class="havok-design-button" href="{{ "/feed.xml" | relative_url }}">
      Subscribe via RSS
    </a>
  </p>
{%- endif -%}