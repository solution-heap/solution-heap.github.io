---
layout: post
title: "Get started"
date: 2025-04-27 00:41:19 +0200
categories: post update
---

Get to know us and what we need from you to able to use the app.

<div class="card-grid">
  {% for post in site.birds %}
  <div class="card">
    <a href="{{post.url|relative_url}}">
      {% if post.image %}
      <img src="{{post.image|relative_url}}" alt="{{post.title}}" />
      {% endif %}
      <h3>{{post.title}}</h3>
      {% if post.excerpt %}
      <p>{{post.excerpt}}</p>
      {% endif %}
    </a>
  </div>
  {% endfor %}
</div>
