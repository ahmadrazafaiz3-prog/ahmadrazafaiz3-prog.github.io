---
layout: post
title: "From Diagrams to Queries: Learning to Actually Talk to a Database"
date: 2026-02-16 09:00:00 +0500
categories: [database, semester-2]
tags: [database, semester-2]
---

![SQL LEFT JOIN query and Venn diagram explanation]({{ "/images/post8-sql-queries.svg" | relative_url }})

> **About the mentor referenced in this post:** Dr. Bilal Ahmad is a Professor at UET Lahore, Faisalabad Campus, and an expert in Artificial Intelligence, Machine Learning, and Deep Learning model training. His name is mentioned throughout this series as he was the instructor who guided and inspired this coursework.
>
> [LinkedIn](https://www.linkedin.com/in/drbilalphd/) · [Google Scholar](https://scholar.google.com.au/citations?user=8nZ0jVkAAAAJ&hl=en) · [Facebook](https://www.facebook.com/Dr.BilalAhm)


After weeks of thinking about databases conceptually through keys and ER diagrams, finally sitting down to write real SQL queries felt like the moment the entire course shifted from theory into something tangible. This topic, more than any other in the Database Systems portion of my semester, gave me the closest thing to the satisfaction I had felt earlier in the semester while writing working Python scripts.

We started, predictably, with basic SELECT statements, pulling specific columns from a single table and applying simple WHERE conditions to filter results. It felt almost too easy at first, similar to how Python's earliest lessons had felt back at the start of the semester. That feeling did not last long. Once we moved into queries involving multiple conditions, combined with AND and OR operators, I quickly learned how easy it is to misplace parentheses and accidentally change the entire logic of a filter without realizing it.

JOIN operations were where this topic genuinely tested me. Understanding the difference between an INNER JOIN and various forms of OUTER JOIN required more than one attempt before it actually made sense. My first real assignment asked us to retrieve a list of students along with the courses they were enrolled in, using the same enrollment scenario we had designed earlier during the ER modeling exercises. I initially used an INNER JOIN without thinking much about it, only to realize during review that any student who had not yet enrolled in a course would be completely missing from my results. Dr. Bilal Ahmad used that exact situation to explain why a LEFT JOIN would have been the more appropriate choice if the goal was to include every student regardless of enrollment status, a distinction that felt minor in theory but turned out to matter enormously in practice.

Aggregate functions, particularly COUNT, AVG, SUM, MIN, and MAX, combined with GROUP BY, were the next significant challenge. The logic of grouping rows together before applying a calculation took some time to internalize, especially when combined with a HAVING clause to filter grouped results, which behaves differently from a WHERE clause in ways that confused me during my first attempt. I distinctly remember trying to use WHERE to filter on an aggregated value and getting an error I did not initially understand, before realizing that WHERE filters rows before grouping while HAVING filters groups after the aggregation has already happened.

Dr. Bilal Ahmad connected this entire topic directly to his work training machine learning models. He explained that before any dataset reaches a model, it almost always passes through a series of SQL queries designed to clean, filter, join, and aggregate raw data into a usable form, and that the medical datasets he prefers working with for their precision often require especially careful queries to avoid accidentally excluding or duplicating patient records during a join. That explanation gave our classroom exercises a sense of real stakes that I had not fully appreciated before.

Subqueries were the most conceptually demanding part of this topic for me. Writing a query inside another query, particularly within a WHERE clause to filter based on a calculated value from a separate query, required a different style of thinking than anything we had done before. I remember spending a noticeably long time on one assignment that asked us to find students whose grade in a specific course was above the average grade for that same course, since it required nesting an aggregate calculation inside a comparison condition. Getting the syntax and logic right on the first attempt felt like a genuine milestone.

INSERT, UPDATE, and DELETE statements rounded out this topic, and while they were syntactically simpler than the SELECT-based queries, they came with their own warning attached clearly by Dr. Bilal Ahmad: an UPDATE or DELETE statement without a properly specified WHERE clause can silently affect every row in a table, a mistake he described as one of the most common and most damaging errors made by inexperienced database users.

By the end of this topic, SQL had stopped feeling like a foreign language and started feeling like a genuinely useful tool, one I could already imagine using well beyond this single course.

This post completes the three pre-midterm Database Systems topics. The next post shifts focus entirely to relational algebra, the formal theoretical foundation that explains, in mathematical terms, exactly what SQL queries are doing behind the scenes.
