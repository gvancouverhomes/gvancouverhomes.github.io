---
layout: default
title: Greater Vancouver Homes
description: Real estate for people who move with intention. Clarity, privacy, real experience. Serving high-value buyers and sellers in Greater Vancouver.
---

<!-- Navigation -->
<nav class="nav">
  <ul>
    <li><a href="{{ '/' | relative_url }}">Home</a></li>
    <li><a href="{{ '/about.html' | relative_url }}">About</a></li>
    <li><a href="{{ '/blog/' | relative_url }}">Blog</a></li>
    <li><a href="{{ '/contact.html' | relative_url }}">Contact</a></li>
    <li><a href="{{ '/search-bridge.html' | relative_url }}">Search Bridge</a></li>
    <li><a href="{{ '/privacy.html' | relative_url }}">Privacy</a></li>
    <li><a href="{{ '/terms.html' | relative_url }}">Terms</a></li>
    <li><a href="{{ '/accessibility.html' | relative_url }}">Accessibility</a></li>
  </ul>
</nav>

<header class="hero">
  <h1>This space is built for people who move with intention.</h1>
  <p>Families who know what matters. Buyers and sellers who value clarity, privacy, and real experience.</p>
</header>

<main>
  <section class="blog-preview">
    <h2>It Starts Here</h2>
    {% assign post = site.posts.first %}
    {% if post %}
      <div class="blog-excerpt">
        <h3><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h3>
        <p>{{ post.excerpt | strip_html | truncatewords: 32 }}</p>
        <a class="read-more" href="{{ post.url | relative_url }}">Read More</a>
      </div>
    {% else %}
      <p>No blog posts found. Stay tuned for updates.</p>
    {% endif %}
  </section>

  <section class="how-i-work-preview">
    <h2>How I Work</h2>
    <p>This isn’t about sales. It’s about alignment.</p>
    <ul>
      <li>The process is steady, not rushed.</li>
      <li>Decisions are made with confidence, not noise.</li>
      <li>Your time, energy, and long-term vision are protected at every step.</li>
    </ul>
  </section>
</main>

<footer>
  <p>&copy; {{ "now" | date: "%Y" }} Greater Vancouver Homes. All rights reserved.</p>
</footer>
