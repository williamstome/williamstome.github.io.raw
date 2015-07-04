---
layout: post
title: "Learning Objectives for an Introductory AI Course"
modified: 2015-06-01
excerpt: "IN WHICH I write new learning objectives for Intro to AI"
tags: [ai, teaching, pedagogy]
image:
  feature: features/AIMA.png
  credit: Artificial Intelligence- A Modern Approach
date: 2015-06-01
comments: true
---

As I've written about in previous posts, I'm going to be co-designing and co-teaching Tufts' "Introduction to Artificial Intelligence" course this fall. When looking over the current syllabus, the first thing I noticed was the stated learning objectives for the course:

> "Description and Objective: This course is an introductory survey of artificial intelligence. The course will cover the history, theory, and computational methods of artificial intelligence. Basic concepts include representation of knowledge and computational methods for reasoning. One or two application areas will be studied, to be selected from expert systems, robotics, computer vision, natural language understanding, and planning."

Among other reasons, this statement is problematic in that it is purely a course description, and doesn't actually specify learning objectives for the course. 

In order to improve this statement, I used a three step process: (1) identify the set of likely student needs and backgrounds, (2) identify my overall course goal given those backgrounds, and (3) craft learning objectives to achieve that goal given those needs.

## Student Needs #

While I'm a scientist (in training), most of the students taking my class will not be traveling that route, for better or for worse. I instead predict that the class will consist of four broad categories of students: (1) computer scientists heading towards graduate school, (2) computer scientists heading towards programming jobs, (3) cognitive & brain scientists, and (4) others (computer scientists who won't continue along routes 1 and 2, and non-majors). The only course prerequisites are Data Structures and Discrete Mathematics, so while I can assume all students have some experience with programming and formal logic, I can't assume experience analyzing algorithms (in particular, with respect to computational complexity), familiarity with search algorithms, or familiarity with probability theory.

## Course Goal ##

I obviously want my students to become familiar with AI techniques. A sub-goal of this is that I want them to become familiar with modern probabilistic AI techniques not currently taught in the course. Since everyone will have programming experience I want them to get experience actually implementing these algorithms, which will be important for those in groups 1 and 2, and possibly those in group 3. If Algorithms were a prerequisite, then I would aim for students to become confident in analyzing and deriving the AI algorithms seen in the course, but that's not the case.

## Learning Objectives ##

The above analyses led me to craft the following three learning objectives.

1. By the end of the semester, students should be able to identify the major classical and modern AI paradigms, and explain how they relate to each other.

1. By the end of the semester, students should be able to analyze the structure of a given problem such that they can choose an appropriate AI paradigm in which to frame that problem.

1. By the end of the semester, students should be able to implement a wide variety of both classical and modern AI algorithms.

If students achieve these objectives, then they should be able to take a given problem, identify and argue for a way in which to frame that problem, and depending on the paradigm (we won't have time to have students implement all the algorithms we cover) be able to easily write a program to solve the problem using the given paradigm.

These learning objectives will undergo revision before they actually end up on the syllabus, and will of course need to be discussed and cleared by my faculty mentor first. In the meantime, I'd appreciate any feedback I can get!

