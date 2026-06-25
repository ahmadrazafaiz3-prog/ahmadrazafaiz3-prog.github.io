---
layout: post
title: "Relational Algebra: Understanding the Math Behind My SQL Queries"
date: 2026-03-09 09:00:00 +0500
categories: [database, semester-2]
tags: [database, semester-2]
---

![Relational algebra operators reference]({{ "/images/post9-relational-algebra.svg" | relative_url }})

> **About the mentor referenced in this post:** Dr. Bilal Ahmad is a Professor at UET Lahore, Faisalabad Campus, and an expert in Artificial Intelligence, Machine Learning, and Deep Learning model training. His name is mentioned throughout this series as he was the instructor who guided and inspired this coursework.
>
> [LinkedIn](https://www.linkedin.com/in/drbilalphd/) · [Google Scholar](https://scholar.google.com.au/citations?user=8nZ0jVkAAAAJ&hl=en) · [Facebook](https://www.facebook.com/Dr.BilalAhm)


Once the midterm exams were behind us, Database Systems took a noticeably different turn. Where the first half of the semester had been focused on practical, hands-on skills like writing keys, drawing ER diagrams, and querying with SQL, the second half opened with something far more theoretical: relational algebra. At first, I was not entirely sure why we needed a formal mathematical notation for operations I had already learned how to perform in SQL. By the end of this topic, I understood exactly why.

Relational algebra represents database operations using a small set of formal operators rather than SQL keywords, and the very first operator we covered, selection, immediately reminded me of a WHERE clause, just expressed using a different symbol and notation. Projection, the operator used to select specific columns rather than rows, mapped directly onto the column-selection part of a SELECT statement. Seeing these direct parallels made the transition feel less intimidating than I had expected going into this topic right after the midterm.

What genuinely challenged me was the union, intersection, and set difference operators, mainly because they required both relations involved in the operation to be union-compatible, meaning they needed to have the same number of columns with matching, comparable data types. I made a mistake early on by trying to apply a set difference operation between two relations that looked similar in name but actually had a different number of attributes, and Dr. Bilal Ahmad used that exact mistake during a review session to explain how this exact kind of incompatibility shows up constantly when combining datasets from different sources, something he deals with regularly when merging multiple medical datasets that were not originally designed with identical structures.

The Cartesian product operator was conceptually simple but practically alarming once I saw it in action. Multiplying every row of one relation against every row of another relation, without any condition narrowing the result, produces an enormous and mostly meaningless result set almost immediately, even with relatively small sample tables. This exercise gave me a much deeper appreciation for why join operations exist in the first place, since a join is essentially a Cartesian product combined with a selection condition that filters out all the meaningless combinations.

The join operator itself, particularly the natural join, was where relational algebra and my earlier SQL knowledge connected most clearly. Working through a natural join exercise by hand, matching rows based on shared attribute values without writing a single line of SQL, made me appreciate just how much logical work a JOIN clause quietly performs behind a single line of code. Dr. Bilal Ahmad pointed out that understanding this underlying logic becomes especially valuable when optimizing slow queries later, since recognizing which relational algebra operations a query is effectively performing can help identify exactly where inefficiency is coming from.

Division was, without question, the most difficult operator covered in this topic. Conceptually, it answers questions like finding entities related to every single value in another set, which sounds straightforward in plain language but required careful, methodical work to apply correctly using the formal notation. I worked through one division exercise involving finding students enrolled in every course offered by a specific department, and it took multiple attempts and a fair amount of scratch paper before the logic finally clicked.

Dr. Bilal Ahmad framed this entire topic as the theoretical backbone that makes database systems trustworthy and predictable. He explained that relational algebra is precisely what allows a database engine to guarantee that a query will return a consistent, mathematically correct result every time, regardless of how the underlying data happens to be structured or stored. Coming from someone who relies on dependable, accurately processed datasets for training machine learning models, that explanation carried real weight.

By the end of this topic, I found myself appreciating SQL differently. It no longer felt like a set of commands to memorize, but like a practical interface built on top of a rigorous mathematical foundation, one designed specifically to guarantee correctness rather than convenience alone.

This post is the first of the two post-midterm Database Systems topics. The next and final post in this series covers normalization, the process of refining a database design to eliminate redundancy and the kinds of problems it inevitably causes.
