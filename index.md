---
layout: home
title: Home
---

# Welcome to My Engineering Journey

Welcome to my personal portfolio blog website. I am a Computer Engineering student at UET Faisalabad. This website serves as my digital footprint where I document my academic journey, learning experiences, projects, and lessons learned throughout my university life. The idea of creating this blog was inspired by my professor, Dr. Bilal Ahmad, who encouraged students to maintain a professional online presence and continuously share their learning experiences.

![My Study Desk](/assets/images/my-study-picture.jpg)

This website documents my learning journey, projects, database systems experience, and university life.

![Database Learning](/assets/images/database-lab.jpg)

I created this portfolio blog following the advice of Dr. Bilal Ahmad to build a professional digital footprint.

![GitHub Work](/assets/images/github-work.jpg)

GitHub Portfolio Website

Throughout this semester, I learned that engineering is not only about attending lectures and passing exams. It is about documenting knowledge, solving real-world problems, and continuously improving technical and communication skills. Through this blog, I aim to share my experiences in Programming Fundamentals, Database Systems, laboratory work, examinations, and personal projects. Writing these posts helps me reflect on what I have learned and preserve valuable lessons for the future.

Database Systems Learning

One of the most memorable parts of this semester was studying Database Systems. We completed three quizzes, a midterm examination, a final examination, several laboratory manuals, and an open-handed laboratory assessment. Before the midterm, we focused on ER modeling, keys, relationships, and SQL queries. After the midterm, we moved toward normalization, relational algebra, and more advanced database concepts. These experiences strengthened my understanding of data organization and management.

University Study Experience

{% for post in site.posts %}

* [{{ post.title }}]({{ post.url }})
  {% endfor %}

