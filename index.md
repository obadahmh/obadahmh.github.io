---
layout: default
title: About
---
<section class="intro">
  <div class="intro-text">
    <h1 class="name">{{ site.author.name }}</h1>
    <p class="role">AI Engineer &middot; Mohamed bin Zayed University of Artificial Intelligence</p>

    <p>I am an AI researcher based in Abu Dhabi, working on deep learning, computer vision and representation learning. I am currently an AI Engineer at <a href="https://mbzuai.ac.ae">MBZUAI</a>, where I work on building biocomputers.</p>

    <p>My recent research focuses on interpretability: neural vision models that are interpretable by design, using concept bottlenecks and sparse autoencoders on top of foundation models such as DINOv2 and CLIP. Before that, my work centred on AI for IoT and UAV systems, including GAN-based source localization and Gaussian process sensor selection.</p>

    <p>I hold an MSc in Electrical and Computer Engineering from Khalifa University and a BSc in Computer Engineering from Abu Dhabi University.</p>

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
