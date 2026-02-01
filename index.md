---
layout: home
title: "Welcome to Breiss Lab"
author_profile: true
header:
  overlay_color: "#000"
  overlay_filter: "0.5"
  overlay_image: /assets/images/header-image.jpg
  caption: "Photo credit: [**Unsplash**](https://unsplash.com)"
excerpt: "Advancing knowledge through cutting-edge research"
---

## About Our Lab

Welcome to the Breiss Lab! We are a research group dedicated to [describe your research focus here]. Our team combines expertise in [research areas] to address fundamental questions in [field of study].

## Research Highlights

Our current research focuses on:

- **Research Area 1**: Brief description of this research direction
- **Research Area 2**: Brief description of this research direction  
- **Research Area 3**: Brief description of this research direction

## Latest News

{% for post in site.posts limit:3 %}
  <article>
    <h3><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h3>
    <p class="post-meta">{{ post.date | date: "%B %d, %Y" }}</p>
    <p>{{ post.excerpt }}</p>
  </article>
{% endfor %}

## Join Us

We are always looking for motivated researchers to join our team. If you're interested in our work, please check our [People](/breisslab/people/) page or [contact us](/breisslab/contact/).
