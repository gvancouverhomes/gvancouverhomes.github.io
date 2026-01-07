---
layout: default
title: Home
description: Helping families move with clarity and confidence.
---

<section class="hero">
  <div class="hero-overlay">
    <div class="hero-text">
      <h1>Tanvir Bhupal</h1>
      <p>
        I work with people who move with intention. Families who know what matters.<br>
        Those who value clarity, privacy, and real experience.
      </p>
    </div>
  </div>
</section>

<section class="intro">
  <div class="container intro-wrap">
    <div class="intro-left">
      <h2>It Starts Here</h2>

      <p class="statement">
        This isn’t about sales. It’s about alignment.<br>
        The process is steady, not rushed.<br>
        Decisions are made with confidence, not noise.<br>
        Your time, energy, and long-term vision are protected at every step.
      </p>

      <a class="read-more" href="/blog/">Insights</a>
    </div>

    <div class="intro-right">
      <h3 class="latest-title">Latest writing</h3>

      {% if site.posts.size > 0 %}
        <div class="latest-grid">
          {% for post in site.posts limit:6 %}
            <a class="post-card" href="{{ post.url }}">
              <div class="post-card-inner">
                <div class="post-title">{{ post.title }}</div>
                {% if post.description %}
                  <div class="post-desc">{{ post.description }}</div>
                {% endif %}
                <div class="post-meta">
                  {{ post.date | date: "%b %e, %Y" }}
                </div>
              </div>
            </a>
          {% endfor %}
        </div>
      {% else %}
        <p class="no-posts">No posts yet. The first one is coming soon.</p>
      {% endif %}
    </div>
  </div>
</section>
