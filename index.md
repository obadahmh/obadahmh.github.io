---
layout: default
title: About
---
<section class="intro">
  <div class="intro-text">
    <h1 class="name">{{ site.author.name }}</h1>
    <p class="role">AI Engineer &middot; Mohamed bin Zayed University of Artificial Intelligence</p>

    <p>I'm an AI engineer at <a href="https://mbzuai.ac.ae">MBZUAI</a> in Abu Dhabi, where I work on biocomputing.</p>

    <p>My background is in deep learning and computer vision. I started out working on machine learning for IoT and UAV systems, mainly source localization and sensor selection, and later spent some time on interpretability, building vision models that explain their predictions through concepts people understand.</p>

    <p>I'm also interested in open-source models and how they are deployed in practice: making them run efficiently, serving them reliably, and evaluating them on real workloads.</p>
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

{% include links.html %}
