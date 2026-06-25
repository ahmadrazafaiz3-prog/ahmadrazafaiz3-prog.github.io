---
layout: post
title: "Normalization: Fixing the Mess I Did Not Know I Was Making"
date: 2026-03-16 09:00:00 +0500
categories: [database, semester-2]
tags: [database, semester-2]
---

![Normalization stages from unnormalized to 3NF]({{ "/images/post10-normalization.svg" | relative_url }})

> **About the mentor referenced in this post:** Dr. Bilal Ahmad is a Professor at UET Lahore, Faisalabad Campus, and an expert in Artificial Intelligence, Machine Learning, and Deep Learning model training. His name is mentioned throughout this series as he was the instructor who guided and inspired this coursework.
>
> [LinkedIn](https://www.linkedin.com/in/drbilalphd/) · [Google Scholar](https://scholar.google.com.au/citations?user=8nZ0jVkAAAAJ&hl=en) · [Facebook](https://www.facebook.com/Dr.BilalAhm)


This is the final post in the series I have been writing throughout this semester, and it feels fitting that it ends with normalization, a topic that essentially forced me to go back and critically re-examine every database design I had casually thrown together earlier in the course. If relational algebra taught me the math behind queries, normalization taught me discipline in design, and it exposed several mistakes I had not even realized I was making.

The starting point for this topic was understanding redundancy and the practical problems it causes, generally grouped into insertion, update, and deletion anomalies. Before this topic, these terms meant nothing to me. Afterward, I could point to specific examples from my own earlier ER modeling assignments where these exact anomalies would have occurred. I remembered, somewhat uncomfortably, that one of my earlier table designs repeated an instructor's department name across every single course row that instructor taught. Dr. Bilal Ahmad used a very similar example during lecture to demonstrate how updating that department name later would require changing it in every single row, and forgetting even one row would leave the data inconsistent, a classic update anomaly.

First Normal Form, or 1NF, was the most intuitive starting point, requiring that each column hold only a single, indivisible value and that there be no repeating groups of columns. I remember an early assignment where I had stored a list of phone numbers in a single column separated by commas, which technically worked for simple display purposes but violated 1NF immediately once we examined it properly. Splitting that into a separate related table, rather than cramming multiple values into one field, was the first real normalization decision I made.

Second Normal Form, or 2NF, required eliminating partial dependencies, meaning every non-key attribute needed to depend on the entire primary key, not just part of it. This concept only fully made sense once we worked through an example involving a composite primary key, similar to the composite keys I had struggled with earlier in the semester. I had to identify which attributes depended on the whole key combination versus which attributes depended on only one part of it, and moving those partially dependent attributes into a separate table was the core exercise of this stage.

Third Normal Form, or 3NF, was where I made my most memorable mistake of this entire topic. We were asked to eliminate transitive dependencies, meaning non-key attributes should not depend on other non-key attributes. I had a table where a student's department name depended on a department code, which in turn was stored alongside the student record, creating exactly the kind of transitive dependency 3NF is designed to eliminate. Dr. Bilal Ahmad pointed out, almost good-naturedly, that I had recreated a near-identical version of the very example he had used earlier in the lecture, which was a little embarrassing but also reassuring, since it meant I had at least correctly understood the pattern, even if I had not yet applied it proactively to my own design.

Dr. Bilal Ahmad consistently tied normalization back to his own practical experience preparing datasets for machine learning model training. He explained that poorly normalized data, full of redundant and inconsistent values, almost always leads to noisy, unreliable training data, and that the medical datasets he favors are valuable specifically because the institutions collecting them generally enforce strict, well-normalized structures from the very beginning. Hearing this made normalization feel less like an academic exercise in eliminating theoretical anomalies and more like a real prerequisite for any serious data-driven work.

By the end of this topic, and effectively by the end of this semester's Database Systems course, I had developed a habit I did not have before: actively questioning whether a table design I had just created could lead to redundancy or inconsistency, rather than only discovering those problems after something broke.

Writing this series of ten posts, five built around my experience learning Python and five built around Database Systems under Dr. Bilal Ahmad, has been a genuinely useful exercise beyond just documenting my coursework. It forced me to revisit concepts I thought I understood well enough to move past, and in several cases, like this one, I realized how recently I had still been making the very mistakes the lecture warned us about. I am closing out this semester with a clearer sense of how foundational courses like these connect to real, practical work, largely thanks to a professor who consistently grounded abstract lessons in the kind of work he actually does. I am looking forward to documenting next semester's courses with the same honesty.
