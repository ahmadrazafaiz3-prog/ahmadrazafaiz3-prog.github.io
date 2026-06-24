---
layout: post
title: "Starting Database Systems: Why Keys Matter More Than I Expected"
date: 2026-2-02 09:00:00 +0500
categories: [database, semester-2]
tags: [database, semester-2]
---

![Primary key and foreign key relationship diagram](/images/post6-database-keys.svg)

Walking into Database Systems this semester, I assumed it would feel similar to Python: a new syntax to learn, a few exercises to complete, and a logical progression from simple to complex. What I did not expect was how much of the course, especially in the early weeks, focused not on syntax at all but on the conceptual backbone of how data should be organized before a single line of SQL is even written. That backbone started with keys, and it turned out to be far more important than I initially gave it credit for.

Dr. Bilal Ahmad, who also taught us Programming Fundamentals in Python, brought a noticeably different energy into this course, shaped heavily by his background in training AI and machine learning models. He made it clear early on that the quality of a database design directly determines the quality of any analysis or model built on top of it later, a point he illustrated repeatedly using examples from medical datasets, which he said he prefers in his own research because of how precisely and accurately they tend to be collected and recorded.

The first real concept that reshaped how I thought about data was the idea of a primary key. Before this course, I thought of a table as just a structured list, similar to a spreadsheet. The idea that every single row needed a unique identifier, one that could never be duplicated and never left empty, felt like an obvious rule once explained but something I had never consciously considered before. We worked through several small exercises identifying which column in a sample table could realistically serve as a primary key, and I quickly learned that "obvious" choices like a person's name are almost never safe candidates, since duplicate names are far more common than people assume.

Foreign keys took longer to fully click. The concept of one table referencing another table's primary key in order to establish a relationship sounded simple in lecture, but understanding why this mattered took an actual exercise to sink in. We were given a scenario involving students and the courses they enrolled in, and asked to design tables that avoided repeating the same student information across multiple rows. My first attempt repeated student details directly inside the enrollment table, which technically worked but duplicated information unnecessarily. Once Dr. Bilal Ahmad pointed out how this duplication becomes a serious problem at scale, especially when updating a single piece of information requires changing it in multiple places, the purpose of foreign keys became far clearer.

Candidate keys and composite keys were the part of this topic that genuinely challenged me. Understanding that a single table could have multiple columns that each independently qualify as a unique identifier, and that sometimes no single column qualifies alone but a combination of two or more columns together does, required redoing a few exercises more than once before the logic settled in my head. Dr. Bilal Ahmad connected this directly to how medical datasets are often structured, where a single patient identifier alone is not always sufficient and a combination of fields, such as patient ID and visit date, may be required to uniquely identify a specific record.

Super keys and the distinction between candidate keys and primary keys felt like a smaller, more technical detail by comparison, but it mattered for understanding exam-style questions that asked us to identify all possible keys in a given table rather than just the one chosen as primary. I found it useful to physically write out every column combination and test uniqueness manually for a few practice tables, rather than trying to reason through it abstractly.

What struck me most by the end of this topic was how much careful thinking happens before any actual querying begins. Dr. Bilal Ahmad repeatedly emphasized that a poorly designed key structure creates problems that no amount of clever SQL can fully fix later, a lesson that initially sounded like a minor warning but increasingly felt like the central theme of the entire course.

This post marks the beginning of the Database Systems portion of my semester. The next post moves into ER modeling, where these abstract ideas about keys and relationships finally get translated into actual diagrams that represent a real-world system.
Dr. Bilal Ahmad (Professor, UET Lahore Faisalabad Campus)

[LinkedIn: ](https://www.linkedin.com/in/drbilalphd/)
[Google Scholar:]( https://scholar.google.com.au/citations?user=8nZ0jVkAAAAJ&hl=en)
[Facebook:]( https://www.facebook.com/Dr.BilalAhm)
