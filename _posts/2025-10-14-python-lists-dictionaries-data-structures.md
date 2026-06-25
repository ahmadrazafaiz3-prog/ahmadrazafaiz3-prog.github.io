---
layout: post
title: "Lists, Dictionaries, and the Moment My Code Started Looking Organized"
date: 2026-01-14 09:00:00 +0500
categories: [python, semester-1]
tags: [python, semester-1]
---

![List vs dictionary vs nested records diagram]({{ "/images/post3-data-structures.svg" | relative_url }})

> **About the mentor referenced in this post:** Dr. Bilal Ahmad is a Professor at UET Lahore, Faisalabad Campus, and an expert in Artificial Intelligence, Machine Learning, and Deep Learning model training. His name is mentioned throughout this series as he was the instructor who guided and inspired this coursework.
>
> [LinkedIn](https://www.linkedin.com/in/drbilalphd/) · [Google Scholar](https://scholar.google.com.au/citations?user=8nZ0jVkAAAAJ&hl=en) · [Facebook](https://www.facebook.com/Dr.BilalAhm)


There is a specific moment in every beginner programmer's journey when scattered variables stop feeling manageable and you realize you desperately need a better way to organize data. For me, that moment arrived right around the time we started working with lists, tuples, dictionaries, and sets in Python. This part of the semester completely changed how I approached every assignment that came after it.

Before this, my code was full of variables like student1, student2, student3, each holding a single piece of information, and any operation that needed to apply across all of them required copy-pasting the same logic three or four times. It was tedious, error-prone, and honestly a little embarrassing once I saw how much cleaner the alternative was. Lists solved that almost instantly. The ability to store a collection of values and loop through them with a single block of code felt like discovering a shortcut that had been hiding in plain sight the whole time.

Dictionaries took a little longer to feel natural. The idea of key-value pairs made sense conceptually, but I kept mixing up when to use a list versus when a dictionary was the better choice. Dr. Bilal Ahmad gave us a comparison that finally made it click: he described a list as a numbered shelf where you find things by position, and a dictionary as a labeled drawer where you find things by name. Given how often his own work involves organizing datasets with labeled features, especially in the medical datasets he prefers because of their precision and accuracy, it made sense that he had such a clear, practical way of explaining the distinction.

One assignment in particular tested our understanding of nested data structures, specifically a list of dictionaries representing multiple records, each with several fields. I remember being intimidated by the assignment description at first glance, mostly because the nesting looked visually complicated. Once I broke it down piece by piece, accessing one dictionary at a time before trying to loop through the whole list, it stopped feeling overwhelming. That experience taught me a lesson that has stayed with me ever since: complexity in code is usually just simplicity stacked several layers deep, and the trick is unstacking it patiently rather than trying to understand everything at once.

Sets were the structure I used the least during assignments, but understanding them mattered for a different reason. Dr. Bilal Ahmad explained how removing duplicate entries efficiently is a constant requirement when cleaning real datasets before feeding them into a model, and sets are often the simplest tool for that exact job. Even though our classroom exercises with sets were small and almost trivial, knowing the real-world motivation behind them made the lesson feel less abstract.

Tuples were a quieter lesson, mostly remembered through one specific mistake. I tried to modify a tuple the same way I would modify a list, and the error message that followed was my first real introduction to the concept of immutability. At the time it felt like an inconvenience, but it eventually made sense as a feature rather than a limitation, especially once we discussed how immutable data can prevent accidental changes to values that are not supposed to change, something that matters a great deal when working with fixed reference data.

By the time this section of the course wrapped up, my assignments looked noticeably different from how they had looked just a few weeks earlier. Instead of dozens of loosely related variables, I was working with structured collections that mirrored how data actually exists in the real world: grouped, labeled, and related to each other. It was the first time I felt like my code resembled something a professional might actually write, even if it was still a small, simple version of that idea.

This stage of the semester also reinforced something Dr. Bilal Ahmad said more than once in class, that the way you structure your data determines how easy or painful everything that comes after will be. At the time it sounded like a small piece of advice. Looking back now, after struggling through assignments where I structured data poorly and assignments where I structured it well, I understand exactly how true that statement is.

The next post in this series moves into object-oriented programming, where I started learning to think not just about organizing data, but about organizing entire pieces of logic into reusable, self-contained units.
