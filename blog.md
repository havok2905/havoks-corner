---
layout: page
title: Blog
permalink: /blog/
---

<p>
  <a class="havok-design-button" href="{{ "/feed.xml" | relative_url }}">
    Subscribe via RSS
  </a>
</p>
{%- if site.posts.size > 0 -%}
  {%- for post in site.posts -%}
    <div>
      <a class="havok-design-system-blog-card" href="{{ post.url | relative_url }}">
        <div class="havok-design-system-blog-card-tags">
          {%- if post.tags.size > 0 -%}
            {%- for tag in post.tags -%}
              <span>{{ tag }}</span>
            {%- endfor -%}
          {%- endif -%}
        </div>
        <div class="havok-design-system-blog-card-content">
          <h3>
            {{ post.title | escape }}
          </h3>
          <p>
            {{ post.excerpt }}
          </p>
        </div>
        <span class="havok-design-system-blog-card-date">
          {%- assign date_format = site.minima.date_format | default: "%b %-d, %Y" -%}
          {{ post.date | date: date_format }}
        </span>
      </a>
    </div>
  {%- endfor -%}
{%- endif -%}