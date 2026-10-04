---
layout: page
title: Writing
permalink: /writing/
---
<p class="lede">Essays, notes and other pieces.</p>

{%- if site.posts.size == 0 %}
<p>Nothing here yet.</p>
{%- endif %}
<ul class="posts">
  {%- for post in site.posts %}
  <li><span class="date">{{ post.date | date: "%b %Y" }}</span><a href="{{ post.url | relative_url }}">{{ post.title }}</a></li>
  {%- endfor %}
</ul>
