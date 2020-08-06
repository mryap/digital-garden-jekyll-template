---
layout: page
title: Home
id: home
permalink: /
---

# Welcome! 🌱

<div class="post-heading">
  <h1 class="post-title">All notes 📘</h1>
  <p style="padding: 3em 1em; background: #f5f7ff; border-radius: 4px;">This is where I post ideas, snippets, resources, thoughts, collections, and other bits and pieces that I find interesting and useful. This is not a showcase and representative of what I can do. The idea is about embracing the idea of curation, by me, for you.🌱</p>
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
          <!-- <div class="sub">{{ entry.excerpt | strip_html }}</div> -->
        </div>
      {% endunless %}
    {% endfor %}
    </div>



<style>
  .wrapper {
    max-width: 46em;
  }
</style>
