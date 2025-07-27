---
layout: default
title: Home
---
<link rel="stylesheet" href="/assets/css/custom.css">
Hi, I'm **Alessandra Amosso**.  
This is a personal blog and notebook where I share ideas, notes, and small software projects :)
### Posts


<link rel="stylesheet" href="/assets/css/custom.css">

<div class="post-list">
  {% for post in site.posts %}
    <div class="post-card">
      <h2><a href="{{ post.url }}">{{ post.title }}</a></h2>
      <p class="post-date">{{ post.date | date: "%B %d, %Y" }}</p>
      {% if post.description %}
        <p>{{ post.description }}</p>
      {% endif %}
    </div>
  {% endfor %}
</div>