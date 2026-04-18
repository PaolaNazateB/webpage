---
layout: default
title: News
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
