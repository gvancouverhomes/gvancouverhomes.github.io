---
layout: default
title: Blog
description: Insights, stories, and perspectives on Greater Vancouver real estate for thoughtful buyers and sellers.
permalink: /blog/
---

<section class="section">
  <h2>Blog</h2>

  <div class="blog-cards">
    {% for post in site.posts %}
      <article class="blog-card">
        <a href="{{ post.url | relative_url }}">
          <img
            src="{{ post.image | default: '/assets/images/blog/placeholder.jpg' | relative_url }}"
            alt="{{ post.title | escape }}">
        </a>

        <div class="blog-card-content">
          <h3><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h3>
          <p>{{ post.description | default: post.excerpt | strip_html | truncate: 140 }}</p>
          <a class="read-more" href="{{ post.url | relative_url }}">Read More</a>
        </div>
      </article>
    {% endfor %}
  </div>
</section>
