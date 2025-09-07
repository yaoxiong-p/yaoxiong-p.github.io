---
layout: default
title: Recent works
---

<div id="recent-works">
  <h1>Recent Works</h1>
  <ul class="posts noList">
    {%- for post in site.posts -%}
      <li style="display:flex; align-items:flex-start; margin-bottom:20px;">
        <div style="flex:1;">
          <span class="date">{{ post.date | date_to_string }}</span>
          <h3 style="margin:4px 0;">
            <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
          </h3>
          <p class="description" style="margin:0;">
            {%- if post.description -%}
              {{ post.description | strip_html | strip_newlines | truncate: 120 }}
            {%- else -%}
              {{ post.content | strip_html | strip_newlines | truncate: 120 }}
            {%- endif -%}
          </p>
        </div>
        {%- if post.image -%}
          <div style="margin-left:16px; flex-shrink:0;">
            <img src="{{ post.image | relative_url }}" 
                 alt="Post image" 
                 style="width:120px; height:auto; border-radius:4px;">
          </div>
        {%- endif -%}
      </li>
    {%- endfor -%}
  </ul>
</div>
