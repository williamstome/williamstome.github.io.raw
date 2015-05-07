---
layout: post
title: "Initial Thoughts on (Re)designing an Introductory AI Course"
modified: 2015-05-07
excerpt: "A month or so ago, I was accepted to the Tufts GIFT (Graduate Institute for Teaching) program"
tags: [ai, teaching, pedagogy]
image:
  feature: features/AIMA.png
  credit: Artificial Intelligence- A Modern Approach
date: 2015-05-07
comments: true
---

A month or so ago, I was accepted to the Tufts GIFT (Graduate
Institute for Teaching) program, which is comprised of (1) a
*learning* portion in which I'll spend three weeks taking classes on
teaching pedagogy, (2) a *design* portion, in which I'll be
working with Professor Anselm Blumer to redesign portions of Tufts'
"Introduction to Artificial Intelligence" course, and (3) a *teaching*
portion, in which I'll teach some number of lectures (I'm hoping
eight) for the redesigned course. 

While I haven't yet undergone the *learning* portion yet, I've been
eager to start brainstorming how I might change the class. 
One complaint many (including myself) have with how the course is
currently structured is that it is has very little of what would be
considered "Modern" AI. In fact, 40% of the class is focused on logic,
which, as I'll show later, is quite a lot. This led me to formulate
my first goal:

> *Classical* and *Modern* AI should be given approximately equal
> weight. 

Another complaint many (including myself) have with how the course is
currently structured is that the course currently seems to just follow
the progression of the textbook, chapter by chapter, without
sufficient motivation for each new topic. This led me to
formulate my second goal:

> Each topic should build off the previous topic in some meaningful
> way. When discussing each new topic, students should have to consider
> how it compares to the previous topics studied.

By thinking about the course in light of these two goals, I
realized that the course material could be nicely organized in the
following way:

* First, there are a set of foundational topics (e.g., *Search* and *Constraint Satisfaction*) that (I believe) sit outside of the Classical/Modern divide
* Second, all the topics I'd like to cover in Classical and Modern AI can be categorized as knowledge representation, inference, or decision making.

|                          | Classical AI                  | Modern AI                                    |
|:-------------------------+:------------------------------+:---------------------------------------------|
| Knowledge Representation | First order Logic, Ontologies | Bayes Nets and Markov Models                 |
|----
| Inference                | First order Logical Inference | Exact and Approximate Inference              |
|----
| Decision Making          | Classical Planning            | Utility Theory and Markov Decision Processes |
{: rules="groups"}

By adding seven classes to the schedule on modern inference and decision
making, cutting six classes on classical knowledge representation
and decision making, and cutting a single class on Foundations, I
constructed the following schedule, which achieves my two goals. I'm
especially excited about the lesson on 
[Markov Logic Nets](http://homes.cs.washington.edu/~pedrod/papers/mlj05.pdf), 
a topic which beautifully ties together Classical and Modern AI.

|----
| Supertopic      | Topic  | Subtopic              |      Old | New |
|:----------------|:-------|:----------------------|:---------|+:----|
| Foundations -1  | Intro  | Introduction          |      1-2 | 1-2 |
| Foundations     | Search | Uninformed Search     |        3 |   3 |
| Foundations     | Search | Heuristic Search      |        4 |   4 |
| Foundations     | Search | Local Search          |        4 |   5 |
| Foundations     | Search | ND Actions            |        5 |   6 |
| Foundations     | Search -1 | Partial Observations  |        6 |   - |
| Foundations     | CSPs   | CSPs                  |        9 |   7 |
| Foundations     | CSPs   | Constraint Prop       |       10 |   8 |
| Foundations     | Search | Adversarial Search    |        7 |   9 |
|----
| Classical AI -6 | KR -5  | FOL                   | 11-15,17 |  10 |
| Classical AI    | KR     | FOL                   |       16 |  11 |
| Classical AI    | Inf    | FOL Inf               |       18 |  12 |
| Classical AI    | Inf    | FOL Inf               |       19 |  13 |
| Classical AI    | KR     | Ontologies            |       24 |  14 |
| Classical AI    | DM -1  | Classical Planning    |    20-22 |  15 |
| Classical AI    | DM     | Hierarchical Planning |        - |  16 |
| Classical AI    | DM     | Other Planning Topics |       23 |  17 |
|----
| Modern AI +7    | KR  +1 | Back to Bayesics      |       25 |  18 |
| Modern AI       | KR     | Bayes Nets            |       26 |  19 |
| Modern AI       | Inf +3 | Exact Inference       |        - |  20 |
| Modern AI       | Inf    | Approx. Inference     |        - |  21 |
| Modern AI       | Inf    | MCs and HMMs          |        - |  22 |
| Modern AI       | KR     | Markov (Logic) Nets   |        - |  23 |
| Modern AI       | DM +3  | Utility Theory        |        - |  24 |
| Modern AI       | DM     | MDPs                  |        - |  25 |
| Modern AI       | DM     | POMDPs                |        - |  26 |
|----
{: rules="groups"}

## Comparison to Other Schools ##

The first question you might ask is whether my proposed cuts are
justified. To examine this, I looked at a random sampling of
universities whose syllabi I could easily find, and looked at the
percentage of the semester each university spent on Foundations
(Search and CSPs), Classical AI (Planning and Logic), and
Modern AI (Probabilistic Graphical Models and Markov Decision Processes).

|------------------+----------------+--------+------+----------+-------+------+------|
| University       | Total Lectures | Search | CSPs | Planning | Logic | PGMs | MDPs |
|:-----------------+:---------------+:-------+:-----+:---------+:------+:-----+:-----|
| Dartmouth        |             27 |   0.19 | 0.07 |        0 |  0.22 | 0.30 |    0 |
| MIT              |             23 |   0.13 | 0.13 |        0 |     0 | 0.09 |    0 |
| Stanford         |             20 |   0.15 |  0.1 |        0 |  0.15 | 0.15 | 0.05 |
| OSU              |             31 |   0.06 |    0 |        0 |  0.06 | 0.26 |    0 |
| WPI              |             26 |   0.08 | 0.04 |     0.04 |  0.04 | 0.19 | 0.04 |
| U of Maine       |             28 |   0.21 | 0.04 |     0.14 |  0.21 | 0.07 |    0 |
| Northeastern     |             29 |   0.10 | 0.03 |     0.03 |  0.14 |    0 |    0 |
| Columbia         |             24 |   0.21 | 0.04 |     0.08 |  0.25 | 0.13 |    0 |
| Berkeley         |             28 |   0.11 | 0.07 |        0 |     0 | 0.29 | 0.04 |
| Georgia Tech     |             32 |   0.13 | 0.03 |     0.06 |  0.03 | 0.13 | 0.06 |
| CMU              |             23 |   0.04 |  0.0 |     0.04 |     0 | 0.22 | 0.09 |
| U Washington     |             27 |   0.22 |    0 |        0 |  0.04 | 0.37 | 0.07 |
| Cornell          |             16 |   0.31 |    0 |        0 | 0.125 |    0 |    0 |
|------------------+----------------+--------+------+----------+-------+------+------|
| AVG              |            ~26 |   0.15 | 0.05 |     0.03 |  0.10 | 0.17 | 0.03 |
| Tufts (Proposed) |             26 |   0.19 | 0.08 |     0.12 |  0.19 | 0.23 | 0.08 |
| Tufts (Current)  |             26 |   0.23 | 0.08 |     0.15 |  0.38 | 0.08 |    0 |
|------------------+----------------+--------+------+----------+-------+------+------|
{: rules="groups"}

This showed that Tufts currently spends slightly more time than
average on Foundations, **four times as much time** on Classical AI,
and 40% as much time on Modern AI. You'll notice that percentages for
most schools falls far short of 100%. This is mainly because most
other schools spend a portion of their AI class on *Machine Learning*,
another facet of Modern AI, which we're explicitly looking to avoid
since we have an entire course devoted to the basics of Machine
Learning. I think it'd be fair to say that we thus spend closer to
20% as much time as other schools on Modern AI once Machine Learning
is taken into account.

## Outlook ##

How much I'll actually be able to modify the course syllabus is still
up in the air, but I'm hoping I'll be able to bring it significantly closer
to my ideal. I'm guessing that MDPs, POMDPs, HMMs and Hierarchical
planning might get the axe in order to add back some of my cuts to the
(egregiously long, in my opinion) section on First Order Logic. Only
time will tell. As this syllabus evolves I'll post regular
updates. And, as always, I'd welcome feedback on this course layout.
