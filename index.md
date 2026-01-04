---
layout: default
title: Home
description: Helping families move with clarity and confidence.
---

<section class="hero">
  <div class="hero-overlay">
    <div class="hero-text">
      <h1>Greater Vancouver Homes</h1>
      <p>
        For people who move with intention. Families who know what matters.<br>
        Buyers and sellers who value clarity, privacy, and real experience.
      </p>
    </div>
  </div>
</section>

<section class="intro">
  <div class="container">
    <h2>It Starts Here</h2>
    <p>This isn’t about sales. It’s about alignment.</p>
    <p>The process is steady, not rushed.</p>
    <p>Decisions are made with confidence, not noise.</p>
    <p>Your time, energy, and long-term vision are protected at every step.</p>
    {% if site.posts.size > 0 %}
  <a class="read-more" href="{{ site.posts.first.url }}">Read More</a>
{% else %}
  <a class="read-more" href="/blog/">Read More</a>
{% endif %}
  </div>
</section>
