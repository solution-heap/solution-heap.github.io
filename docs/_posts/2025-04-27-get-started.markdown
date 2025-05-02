---
layout: post
title: "Get started"
date: 2025-04-27 00:41:19 +0200
categories: post update
---

Get to know us and what we need from you to able to use the app.

<style>
.card{
    background-color: #f9f9f9;
    border-radius: 8px;
    box-shadow: 0 2px 4px rgba(0,0,0,0.1);
    overflow: hidden;
   
}

.card h3{
    margin-top: 0;
    margin-bottom: 10px;
}
.card p {
    margin: 10px;
    padding: 20px;
    
}
</style>

<div class="card">
  {% for post in site.birds %}
  <div>
    <a href="{{post.url|relative_url}}">
      <p>{{post.title}}</p>
    </a>
  </div>
  {% endfor %}
</div>
