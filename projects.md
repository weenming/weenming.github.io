---
layout: page
title: Projects
permalink: /projects/
---

<header class="post-header">
<h1 class="post-title">{{ page.title | escape }}</h1>
</header>

<ul class="post-list">
{%- for post in site.posts -%}
    {% if post.type == "project" %} 
    <!-- display only the blog type posts -->
    <li>
        {%- assign date_format = site.minima.date_format | default: "%b %-d, %Y" -%}
        <span class="post-meta">{{ post.date | date: date_format }}</span>
        <h3>
        <a class="post-link" href="{{ post.url | relative_url }}">
            {{ post.title | escape }}
        </a>
        </h3>
        {%- if site.show_excerpts -%}
        {{ post.excerpt }}
        {%- endif -%}
    </li>
    {% endif %}
{%- endfor -%}
</ul>

