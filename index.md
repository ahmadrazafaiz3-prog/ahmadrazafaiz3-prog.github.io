---
layout: home
title: Home
---

# Welcome to My Engineering Journey

I am Ahmad Raza, a Computer Engineering student at UET Faisalabad.

![My Study Desk](/assets/images/my-study-picture.jpg)

This website documents my learning journey, projects, database systems experience, and university life.

![Database Learning](/assets/images/database-lab.jpg)

I created this portfolio blog following the advice of Dr. Bilal Ahmad to build a professional digital footprint.

![GitHub Work](/assets/images/github-work.jpg)

Here you can find my blog posts, study experiences, and technical projects.
---

{% for post in site.posts %}

* [{{ post.title }}]({{ post.url }})
  {% endfor %}

