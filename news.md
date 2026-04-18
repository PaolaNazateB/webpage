---
layout: default
title: Talks and Conferences
permalink: /news/
---

<h2>News</h2>

<ul>
  {% for item in site.news %}
    <li>
      <strong>{{ item.date | date: "%Y-%m-%d" }}</strong> —
      {{ item.title }}
      <br>
      {{ item.content }}
    </li>
  {% endfor %}
</ul>


<a href="{{ '/' | relative_url }}" class="btn btn-light btn-sm mb-3">
    ← Back to Home
</a>
