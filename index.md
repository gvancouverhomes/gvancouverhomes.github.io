---
layout: default
title: Tanvir Bhupal
description: For people who move with intention. Clarity, privacy, and real experience for families relocating in Greater Vancouver.
permalink: /
---

<script type="application/ld+json">
{
  "@context": "https://schema.org",
  "@type": "WebPage",
  "name": "Tanvir Bhupal",
  "description": "For people who move with intention. Clarity, privacy, and real experience for families relocating in Greater Vancouver.",
  "url": "https://tanvirbhupal.com/",
  "inLanguage": "en-CA"
}
</script>

<section class="hero">
  <div class="hero-content">
    <h1>For people who move with intention</h1>
    <p>
      Families who know what matters.<br>
      Those who value clarity, privacy, and real experience.
    </p>

    <p class="visually-hidden">
      Real estate insights for families relocating across Greater Vancouver, including Vancouver, West Vancouver, North Vancouver, Surrey, South Surrey, and White Rock.
    </p>
  </div>
</section>

<section class="section intro-wide">
  <div class="container">
    <h2>It Starts Here</h2>

    <p class="statement">
      This isn’t about sales. It’s about alignment.<br>
      The process is steady, not rushed.<br>
      Decisions are made with confidence, not noise.<br>
      Your time, energy, and long-term vision are protected at every step.
    </p>

    <a class="read-more" href="/blog/">Insights</a>
  </div>
</section>


<section class="section latest-insights">
  <h2>Latest Insights</h2>

  <div class="blog-cards">
    {% for post in site.posts limit:3 %}
      <a class="blog-card" href="{{ post.url | relative_url }}">
        <img
          src="{{ post.image | relative_url }}"
          alt="{{ post.title | escape }}">

        <div class="blog-card-content">
          <h3>{{ post.title }}</h3>
          <p>{{ post.description | default: post.excerpt | strip_html | truncate: 120 }}</p>
        </div>
      </a>
    {% endfor %}
  </div>
</section>
