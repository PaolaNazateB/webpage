---
layout: default
title: Talks and Conferences
permalink: /talks/
---

<a href="{{ '/' | relative_url }}" class="btn btn-light btn-sm mb-3">
  ← Back to Home
</a>

<h2>Talks and Conferences</h2>

{% assign talks = site.news | sort: "date" | reverse %}
<ul>
  {% for item in talks %}
    <li>
      <strong>{{ item.date | date: "%Y-%m-%d" }}</strong> —
      {{ item.title }}
      <br>
      {{ item.content }}
    </li>
  {% endfor %}
</ul>
