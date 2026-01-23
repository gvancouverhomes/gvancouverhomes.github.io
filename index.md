---
layout: default
title: Home
description: Helping families move with clarity and confidence.
---

<section class="hero">
  <div class="hero-content">
    <h1>For people who move with intention</h1>
    <p>
      Families who know what matters.<br>
      Those who value clarity, privacy, and real experience.
    </p>
  </div>
</section>

<section class="section">
  <h2>It Starts Here</h2>

  <p class="statement">
    This isn’t about sales. It’s about alignment.<br>
    The process is steady, not rushed.<br>
    Decisions are made with confidence, not noise.<br>
    Your time, energy, and long-term vision are protected at every step.
  </p>

  <a class="read-more" href="/blog/">Insights</a>
</section>

<section class="section">
  <h2>Latest Insights</h2>

  <div class="blog-cards">
    {% for post in site.posts limit:2 %}
      <article class="blog-card">
        <a href="{{ post.url | relative_url }}">
          <img
            src="{{ post.image | default: '/assets/images/blog/placeholder.jpg' | relative_url }}"
            alt="{{ post.title | escape }}">
        </a>

        <div class="blog-card-content">
          <h3><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h3>
          <p>{{ post.description | default: post.excerpt | strip_html | truncate: 120 }}</p>
          <a class="read-more" href="{{ post.url | relative_url }}">Read More</a>
        </div>
      </article>
    {% endfor %}
  </div>
</section>
