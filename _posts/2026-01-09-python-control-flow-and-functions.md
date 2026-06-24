---
layout: post
title: "Control Flow and Functions: Where Python Finally Clicked For Me"
date: 2026-01-09 09:00:00 +0500
categories: [python, semester-1]
tags: [python, semester-1]
---

![Flowchart of a grade-classification conditional](/images/post2-control-flow-functions.svg)

If my first encounter with Python was about learning the alphabet of programming, this stage of the semester was about learning to form sentences. Control flow, conditionals, loops, and functions turned out to be the part of the course where everything I had learned earlier finally started fitting together into something that felt like actual problem-solving.

The first real challenge came with nested conditionals. I remember staring at an exercise that asked us to classify a student's grade based on multiple ranges, and somehow managing to write a working solution that was almost embarrassingly long because I had not yet learned to simplify my logic. It worked, but it was clunky. It was only after a review session that I understood how to collapse those nested if-else chains into something cleaner using elif statements. That single change made my code about half as long and far easier to read.

Loops were where I had my biggest "aha" moment of the semester so far. Writing a for loop to iterate through a list felt natural almost immediately, but while loops took longer to feel intuitive, mostly because I kept forgetting to update my loop condition variable and ended up with a few infinite loops that froze my terminal. I will admit I panicked the first time it happened, convinced I had broken something. A classmate reminded me that Ctrl+C exists, and I felt simultaneously relieved and a little silly.

Dr. Bilal Ahmad used this exact stage of the course to introduce a concept that stuck with me: the idea of "computational thinking before code." He repeatedly told us that before writing a single line, we should be able to describe the logic of a loop or condition in plain language, almost like writing instructions for a person rather than a machine. Given that he spends much of his own work training machine learning models, often on medical datasets where a logic error can have real consequences, it made sense why he was so insistent on this habit. He was not just teaching Python syntax; he was teaching a way of thinking that he clearly uses in his own research.

Functions were the next big shift, and this is where I started to feel like a real programmer rather than someone just following along with examples. Understanding parameters, return values, and the difference between a function that prints something and a function that returns something took a few tries to fully sink in. I distinctly remember submitting an assignment where every function printed its result instead of returning it, which worked fine in isolation but completely broke when I tried to use those functions together in a larger program. That mistake taught me more about how real programs are structured than any lecture slide could have.

We were also introduced to the idea of default parameters and variable-length arguments, which felt like unnecessary complexity at first but turned out to be incredibly useful once I started writing functions that needed to handle a flexible number of inputs. Dr. Bilal Ahmad mentioned that this kind of flexibility is exactly what makes Python so well suited to building data processing functions that need to work across different dataset shapes and sizes, something he deals with constantly when preparing data for model training.

By the time we reached the end of this section, I had written enough small functions that I started recognizing patterns across my own assignments. A function to validate input. A function to compute a statistic. A function to format output. I began to see programming less as a series of isolated problems and more as a toolkit of small, dependable pieces that could be combined in different ways.

One evening, while debugging a recursive function for a factorial calculation, I finally understood what people mean when they describe debugging as "satisfying." I had been stuck for almost two hours on a logic error, certain my recursive case was correct, only to realize my base case was checking the wrong condition. The moment I fixed it and watched the correct output print was genuinely one of my favorite moments of the semester.

This stretch of the course did not just teach me syntax. It taught me patience, the value of breaking problems into smaller pieces, and a working respect for how much thinking should happen before typing. The next post in this series moves into data structures, lists, dictionaries, and the kind of organization that turns scattered variables into something resembling real data.
[Dr. Bilal Ahmad] (Professor, UET Lahore Faisalabad Campus)
[LinkedIn:]( https://www.linkedin.com/in/drbilalphd/)
[Google Scholar:]( https://scholar.google.com.au/citations?user=8nZ0jVkAAAAJ&hl=en)

