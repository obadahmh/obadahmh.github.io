---
layout: default
title: About
---
<section class="intro">
  <div class="intro-text">
    <h1 class="name">{{ site.author.name }}</h1>
    <p class="role">AI Engineer &middot; Mohamed bin Zayed University of Artificial Intelligence</p>

    <p>I'm an AI engineer at <a href="https://mbzuai.ac.ae">MBZUAI</a> in Abu Dhabi. These days I'm part of a team building biocomputers.</p>

    <p>Most of my research has been about interpretability. I want models whose decisions I can actually inspect, so I've spent the last couple of years building vision models that are interpretable by design, using concept bottlenecks and sparse autoencoders on top of models like DINOv2 and CLIP. Before that I worked on AI for IoT and drones: locating radiation sources with GANs, and deciding which sensors to listen to with Gaussian processes.</p>

    <p>I'm also interested in open-source models and what it takes to put them to use. That means getting them to run well on the hardware people actually have, serving them reliably, and checking that they still hold up once they leave the benchmark.</p>

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
