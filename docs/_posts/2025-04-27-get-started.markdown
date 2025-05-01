---
layout: post
title: "Get started"
date: 2025-04-27 00:41:19 +0200
categories: post update
---

Get to know us and what we need from you to able to use the app.

<div>
    {% for bird in site.birds %}
        <a href="{{bird.url}}">
        {{bird.title}}
        </a>
    {% endfor %}
</div>
    

Test stuff.
