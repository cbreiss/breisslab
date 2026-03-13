---
layout: home
title: "Breiss Lab"
author_profile: true
header:
  overlay_color: "#000"
  overlay_filter: "0.5"
excerpt: "Computational and Experimental Linguistics at USC"
---

## About the Lab

The Breiss Lab is based in the [USC Linguistics Department](https://dornsife.usc.edu/ling/) at the University of Southern California. We study phonology — the sound systems of human language — using computational modeling, corpus methods, and behavioral experiments.

Our research addresses questions about how phonological knowledge is represented and learned, how phonology interacts with morphosyntax and the lexicon, and how overlapping and interacting phonological processes are structured.

## Research Interests

- **Learning & acquisition** — how phonological generalizations are acquired from input
- **Phonological representations** — the structure of overlapping and interacting processes
- **Interfaces** — phonology's interactions with morphosyntax and the lexicon
- **Methods** — Bayesian modeling, corpus methods, online experiments, laboratory phonology

## Latest News

{% for post in site.posts limit:3 %}
  <article>
    <h3><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h3>
    <p class="post-meta">{{ post.date | date: "%B %d, %Y" }}</p>
    <p>{{ post.excerpt }}</p>
  </article>
{% endfor %}

## Join Us

We welcome inquiries from prospective students and collaborators. See the [People](/people/) page or [contact us](/contact/).
