---
layout: default
title: About
---
<section class="intro">
  <div class="intro-text">
    <h1 class="name">{{ site.author.name }}</h1>
    <p class="role">Role &middot; Institution</p>

    <p>A short paragraph introducing yourself: what you work on, where, and why it matters. This is placeholder text that will be replaced with content from your CV.</p>

    <p>A second paragraph on research interests, current projects, or what you are looking for next.</p>

    {% include links.html %}
  </div>
</section>

<section>
  <h2>News</h2>
  <ul class="news">
    {%- for item in site.data.news limit: 5 %}
    <li><span class="date">{{ item.date | date: "%b %Y" }}</span><span>{{ item.text | markdownify | remove: '<p>' | remove: '</p>' }}</span></li>
    {%- endfor %}
  </ul>
</section>

<section>
  <h2>Selected publications</h2>
  <ul class="pubs">
    {%- for pub in site.data.publications %}{% if pub.selected %}
    {% include publication.html pub=pub %}
    {%- endif %}{% endfor %}
  </ul>
  <p class="more"><a href="{{ '/publications/' | relative_url }}">All publications &rarr;</a></p>
</section>

{%- if site.posts.size > 0 %}
<section>
  <h2>Recent writing</h2>
  <ul class="posts">
    {%- for post in site.posts limit: 3 %}
    <li><span class="date">{{ post.date | date: "%b %Y" }}</span><a href="{{ post.url | relative_url }}">{{ post.title }}</a></li>
    {%- endfor %}
  </ul>
</section>
{%- endif %}
