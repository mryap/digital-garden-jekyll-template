---
layout: page
title: Home
id: home
permalink: /
---

# Welcome! 🌱

<div class="post-heading">
  <h1 class="post-title">All notes 📘</h1>
  <p>I'm experimenting with maintaining a public graph of notes to foster an environment where thoughts collide, in a way that I can build upon the combination of ideas. Kind of like a digital garden, with small seedlings that eventually grow into mature trees. 🌱</p>
</div>

<!-- <p style="padding: 3em 1em; background: #f5f7ff; border-radius: 4px;">
  Take a look at <span style="font-weight: bold">[[Your first seed]]</span> to get started on your exploration.
</p> -->

<div>
    {% assign notes = site.notes | where_exp: "item", "item.path contains 'notes'" | sort: "date" | reverse %}
    {% for entry in notes %}
      {% unless entry.path contains "index.md" or entry.path contains "index.html" %}
        {% assign currentdate = entry.last_modified_at | date: "%B %Y" %}
        {% if currentdate != date %}
          {% assign date = currentdate %}
          <div class="super">Last updated in {{ date }}</div>
        {% endif %}
        <div class="blog-entry">
          <a class="internal-link" href="{{ entry.url }}">{{entry.title | replace: '_notes', '/notes' }}</a>
          <div class="sub">{{ entry.excerpt | strip_html }}</div>
        </div>
      {% endunless %}
    {% endfor %}
    </div>

This digital garden template is free, open-source, and [available on GitHub here](https://github.com/maximevaillancourt/digital-garden-jekyll-template).

The easiest way to get started is to read this [step-by-step guide explaining how to set this up from scratch](https://maximevaillancourt.com/blog/setting-up-your-own-digital-garden-with-jekyll). If you need any help, my [DMs are open on Twitter (@vaillancourtmax)](https://twitter.com/vaillancourtmax). Say hi! 👋

<style>
  .wrapper {
    max-width: 46em;
  }
</style>
