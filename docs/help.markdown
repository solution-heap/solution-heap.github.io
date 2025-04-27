---
layout: post
title: Help
permalink: /help/
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

<div class="card-grid">
  {% for post in site.posts %}
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
