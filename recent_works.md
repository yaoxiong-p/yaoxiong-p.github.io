---
layout: default
title: Recent works
---

<div id="recent-works">
  <h1 class="recent-title">Recent Works</h1>
  <ul class="posts noList">
    {%- for post in site.posts -%}
      <li style="display:flex; align-items:flex-start; margin-bottom:24px; gap:20px;">
        <div style="flex:2;">
          <span class="date" style="font-size:0.9em; color:#666;">
            {{ post.date | date_to_string }}
          </span>
          <h3 style="margin:4px 0; font-size:1em; font-weight:600;">
            <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
          </h3>
          <p class="description" style="margin:0; font-size:0.95em; line-height:1.4;">
            {%- if post.description -%}
              {{ post.description | strip_html | strip_newlines | truncate: 120 }}
            {%- else -%}
              {{ post.content | strip_html | strip_newlines | truncate: 120 }}
            {%- endif -%}
          </p>
        </div>
        {%- if post.image -%}
          <div style="flex:1; max-width:33%;">
            <img src="{{ post.image | relative_url }}" 
                 alt="Post image" 
                 style="width:100%; height:auto; border-radius:6px;">
          </div>
        {%- endif -%}
      </li>
    {%- endfor -%}
  </ul>
</div>

<style>
  .recent-title {
    font-size: 1.8rem;
    font-weight: 700;
    margin-bottom: 1.5rem;
  }
</style>
