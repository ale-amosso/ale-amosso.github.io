---
layout: default
title: Home
---

Hi, I'm **Alessandra Amosso**.  
This is a personal blog and notebook where I share ideas, notes, and small software projects :)
### Posts

<ul>
  {% for post in site.posts %}
    <li>
      <a href="{{ post.url }}">{{ post.title }}</a> ({{ post.date | date: "%Y-%m-%d" }})
    </li>
  {% endfor %}
</ul>
