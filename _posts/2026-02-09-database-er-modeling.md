---
layout: post
title: "Drawing Before Building: My Experience With ER Modeling"
date: 2026-02-09 09:00:00 +0500
categories: [database, semester-2]
tags: [database, semester-2]
---

![ER diagram of Student-Enrolls-Course relationship]({{ "/images/post7-er-modeling.svg" | relative_url }})

> **About the mentor referenced in this post:** Dr. Bilal Ahmad is a Professor at UET Lahore, Faisalabad Campus, and an expert in Artificial Intelligence, Machine Learning, and Deep Learning model training. His name is mentioned throughout this series as he was the instructor who guided and inspired this coursework.
>
> [LinkedIn](https://www.linkedin.com/in/drbilalphd/) · [Google Scholar](https://scholar.google.com.au/citations?user=8nZ0jVkAAAAJ&hl=en) · [Facebook](https://www.facebook.com/Dr.BilalAhm)


If learning about keys taught me why structure matters in a database, learning ER modeling taught me how to actually plan that structure before writing a single table definition. This was, without question, one of the most visually engaging topics of the entire semester, mostly because it finally gave us a way to draw out the ideas we had only discussed abstractly in earlier weeks.

Entity-Relationship modeling, or ER modeling, starts with identifying entities, the real-world objects or concepts a database needs to represent, such as students, courses, or instructors. This part felt intuitive almost immediately, since identifying "things" in a system is not too different from identifying nouns in a sentence. The harder part came with identifying attributes correctly, particularly distinguishing between attributes that belong directly to an entity versus attributes that actually describe a relationship between two entities.

Our first major exercise asked us to design an ER diagram for a simplified university enrollment system. I remember confidently sketching out Student and Course as entities, only to get stuck when trying to figure out where to place the "grade" attribute. My instinct was to attach it to the Student entity, since a grade seemed like something that belonged to a student. Dr. Bilal Ahmad corrected this gently but clearly during a review session, explaining that a grade actually depends on the specific combination of a student and a course, not on the student alone, which meant it belonged on the relationship itself rather than on either entity individually. That single correction completely changed how I thought about the rest of the diagram.

Relationships and their cardinalities were the next major hurdle. Understanding the difference between one-to-one, one-to-many, and many-to-many relationships sounds simple when explained in a sentence, but translating a real scenario into the correct cardinality required more careful thinking than I expected. The enrollment system example again became useful here, since a student can enroll in many courses and a course can have many students enrolled, making it a clear many-to-many relationship, which Dr. Bilal Ahmad pointed out would eventually require its own separate table once we moved from diagram to implementation.

Dr. Bilal Ahmad consistently tied these exercises back to his own work with real datasets. He explained that before he ever begins training a machine learning model on a medical dataset, he spends significant time understanding how different entities in the data relate to each other, such as how a single patient might relate to multiple visits, and how each visit might relate to multiple recorded measurements. Hearing this made our classroom exercise feel less like an academic formality and more like a small-scale version of work actually being done in research.

Weak entities were a concept that initially confused me, mainly because the terminology made them sound less important, when in reality they simply describe entities that cannot be uniquely identified without relying on another entity's key. Our example involved a Dependent entity tied to an Employee entity, where a dependent could not be uniquely identified without knowing which employee they belonged to. Drawing the correct notation for this, with the appropriate double-lined boxes and identifying relationships, took a few attempts to get exactly right.

Generalization and specialization, the idea of grouping similar entities under a more general entity or splitting a general entity into more specific subtypes, felt like a natural extension of the inheritance concept I had just learned in Python's object-oriented programming module. I distinctly remember the moment I noticed the parallel myself, before anyone in class pointed it out, and it gave me a small but genuine sense of satisfaction to see two completely different courses reinforcing the same underlying idea from different angles.

By the time we finished this topic, sketching out an ER diagram for a new scenario felt far less intimidating than it had at the start. I started to appreciate ER modeling not as a separate, optional planning step, but as the actual foundation that determines whether everything built afterward will hold together properly.

This post covers the second of three pre-midterm Database Systems topics. The next post moves from diagrams into actual implementation, covering the SQL queries that bring an ER design to life inside a real database.
