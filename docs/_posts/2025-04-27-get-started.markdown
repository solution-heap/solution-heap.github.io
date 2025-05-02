---
layout: post
title: "Get started"
date: 2025-04-27 00:41:19 +0200
categories: post update
---

<style>
  .card-grid{
    display: grid;
    grid-template-columns: repeat(auto-fit,minmax(300px,1fr));
    gap: 20px;
    padding: 20px;
}
.card{
    background-color: #f9f9f9;
    border-radius: 8px;
    box-shadow: 0 2px 4px rgba(0,0,0,0.1);
    overflow: hidden;
    transition: transform 0.3s ease-in-out;
    &:hover{
      transform: scale(1.05);

    }
}

.card a{
    display: block;
    text-decoration: none;
    color: inherit;
    padding: 20px;

}
.card img{
width: 100%;
height: auto;
display: block;
border-bottom: 1px solid #eee;
}
.card h3{
    margin-top: 0;
    margin-bottom: 10px;
}
.card p {
    margin-bottom: 0;
    color: #555;
}
</style>

Get to know us and what we need from you to able to use the app.

<div class="card">
  {% for post in site.birds %}
  <div >
    <a href="{{post.url|relative_url}}">
      <h3>{{post.title}}</h3>
    </a>
  </div>
  {% endfor %}
</div>
