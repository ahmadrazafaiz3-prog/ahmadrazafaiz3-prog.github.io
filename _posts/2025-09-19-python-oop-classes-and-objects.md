---
layout: post
title: "Classes, Objects, and Thinking in Blueprints"
date: 2026-01-19 09:00:00 +0500
categories: [python, semester-1]
tags: [python, semester-1]
---

![Vehicle, Car, and Bike class inheritance diagram]({{ "/images/post4-oop-basics.svg" | relative_url }})

> **About the mentor referenced in this post:** Dr. Bilal Ahmad is a Professor at UET Lahore, Faisalabad Campus, and an expert in Artificial Intelligence, Machine Learning, and Deep Learning model training. His name is mentioned throughout this series as he was the instructor who guided and inspired this coursework.
>
> [LinkedIn](https://www.linkedin.com/in/drbilalphd/) · [Google Scholar](https://scholar.google.com.au/citations?user=8nZ0jVkAAAAJ&hl=en) · [Facebook](https://www.facebook.com/Dr.BilalAhm)


Object-oriented programming was the topic I was most nervous about going into this semester, mostly because every senior student I had asked about it described it as "a different way of thinking" without ever explaining what that actually meant. Now that I have gone through it myself, I finally understand what they meant, and I want to document it here while the experience is still fresh.

The shift started with the simplest possible idea: a class is a blueprint, and an object is something built from that blueprint. It sounds almost too simple to matter, but the implications took a while to sink in. Up until this point, every program I had written treated data and the functions that operated on that data as separate things. Suddenly, classes were asking me to bundle them together, with attributes representing data and methods representing behavior, all living inside the same structure.

My first class assignment involved modeling a simple student record, with attributes like name, registration number, and grades, along with methods to calculate a GPA. It seemed straightforward on paper, but I hit a wall almost immediately because I forgot to include self as the first parameter in my methods. The error messages were confusing at first, and I spent longer than I would like to admit trying to figure out why Python kept complaining about missing arguments I was sure I had provided. Once I understood that self refers to the specific object calling the method, everything about the syntax suddenly made sense.

Dr. Bilal Ahmad framed object-oriented programming in a way that connected directly to his own work training machine learning models. He explained that when building and experimenting with models, especially across different medical datasets, it becomes far more manageable to define a class that encapsulates a model's configuration, training method, and evaluation logic, rather than scattering related functions and variables across a script. Hearing that helped me understand why this paradigm exists beyond academic exercises. It was not just a new syntax to memorize; it was a structural decision that makes large codebases easier to manage and extend.

Constructors, specifically the __init__ method, were another concept that took a few attempts to fully understand. I remember writing a class where I defined attributes outside the constructor by mistake, which technically worked but meant every object I created shared the same values unless I explicitly changed them. That mistake led to a confusing debugging session where changing one object's attribute seemed to affect another object entirely. Dr. Bilal Ahmad used that exact kind of mistake as a teaching example, explaining how subtle bugs like this are exactly the kind of thing that can silently corrupt experiments if you are not careful, particularly when working with multiple model instances trained on different data subsets.

Inheritance was the concept that genuinely impressed me once I understood it. Being able to define a general class and then create more specific versions of it without rewriting shared logic felt like one of the most elegant ideas I had encountered in the course so far. I built a small example with a general Vehicle class and more specific Car and Bike subclasses, and the satisfaction of watching shared methods work correctly across both subclasses, while still allowing each one to have its own specific behavior, was genuinely rewarding.

Encapsulation took longer to appreciate because its benefits are not always visible in small classroom exercises. It was only when Dr. Bilal Ahmad described how protecting internal data of a class prevents external code from accidentally corrupting it, similar to how a trained model's internal parameters should not be casually modified by code outside the training process, that the concept felt genuinely important rather than just an academic rule to follow.

By the end of this topic, I noticed a real shift in how I approached new problems. Instead of immediately thinking about variables and functions, I started asking myself what kind of "thing" I was modeling and what behaviors that thing should have. That shift in thinking, more than any specific syntax, is what I consider the real achievement of this stage of the semester.

This post wraps up the core Python programming topics from this semester. The next post shifts gears completely, moving away from concepts and into the chaos of exam week itself, a stretch of the semester that tested patience far more than it tested programming skill.
