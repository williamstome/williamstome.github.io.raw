---
layout: post
title: "(Re)designing an Introductory AI Course: Post-Semester Analysis"
modified: 2016-02-05
excerpt: "IN WHICH I compare my planned AI course to reality."
tags: [ai, teaching, pedagogy]
image:
  feature: features/AIMA.png
  credit: Artificial Intelligence- A Modern Approach
date: 2016-02-05
comments: true
---

In the Fall of 2015, I was given the opportunity to co-teach Tufts'
Artificial Intelligence class, through Tufts GIFT (Graduate 
Institute for Teaching) program. As I described in
[this pre-class blog post](http://williamstome.github.io//initial-thoughts-on-re-designing-an-introductory-ai-course/),
I took the opportunity to re-design the 
class in order to include more topics from "Modern" (i.e.,
probabilistic AI). As described in that blog post, I had grand plans,
but had no idea to what extent I'd be able to implement them. 
Let's look at how Tom's grand plan worked out!

|----
| Supertopic      | Topic  | Subtopic              |      Old | Planned | Actual |
|:----------------|:-------|:----------------------|:---------|+:----------|+:----------|
| Foundations   | Intro  | Introduction          |      1-2 | 1-2 | 1-2|
| Foundations     | Search | Uninformed Search     |        3 |   3 |3|
| Foundations     | Search | Heuristic Search      |        4 |   4 |4|
| Foundations     | Search | Local Search          |        4 |   5 |5|
| Foundations     | Search | ND Actions            |        5 |   6 |10|
| Foundations     | Search  | Partial Observations  |        6 |   - |-|
| Foundations     | CSPs   | CSPs                  |        9 |   7 |6|
| Foundations     | CSPs   | Constraint Prop       |       10 |   8 |7|
| Foundations     | Search | Adversarial Search    |        7 |   9 |9|
|----
| Classical AI  | KR   | FOL                   | 11-15,17 |  10 |11|
| Classical AI    | KR     | FOL                   |       16 |  11 |12|
| Classical AI    | Inf    | FOL Inf               |       18 |  12 |13|
| Classical AI    | Inf    | FOL Inf               |       19 |  13 |14|
| Classical AI    | KR     | Ontologies            |       24 |  14 |15|
| Classical AI    | DM   | Classical Planning    |    20-22 |  15 |16|
| Classical AI    | DM     | Hierarchical Planning |        - |  16 |24|
| Classical AI    | DM     | Other Planning Topics |       23 |  17 |20,22|
|----
| Modern AI     | KR   | Back to Bayesics      |       25 |  18 |8|
| Modern AI       | KR     | Bayes Nets            |       26 |  19 |17|
| Modern AI       | Inf  | Exact Inference       |        - |  20 |18-19|
| Modern AI       | Inf    | Approx. Inference     |        - |  21 |21|
| Modern AI       | Inf    | MCs and HMMs          |        - |  22 |(21)|
| Modern AI       | KR     | Markov (Logic) Nets   |        - |  23 |23|
| Modern AI       | DM   | Utility Theory        |        - |  24 |(8)|
| Modern AI       | DM     | MDPs                  |        - |  25 |25|
| Modern AI       | DM     | POMDPs                |        - |  26 |-|
| Modern AI       | DM     | Factored MDPs         |        - |  - |26|
|----
{: rules="groups"}

## Outcome ##

Two things should immediately stand out by comparing the last three
columns of the chart above.  

First, I was successful in convincing my co-instructor, Prof. Anselm
Blumer, to shift most of the sessions on Logic to topics from Modern
AI. This was a big surprise for me, as I initially had no idea whether
or not he'd be receptive to such a major shift. We ended up dropping
HMMs and POMDPs and picking up Factored MDPs, but otherwise the topics
covered were just what I'd hoped for.  

Second, though, you'll notice that the actual class schedule jumped
around **a lot**. For example, the last section of the course (16-26)
went: **Planning**, Bayes Nets, Bayesian Inference, Bayesian Inference,
**Planning**, Bayesian Inference, **Planning**, Markov Logic,
**Planning**, MDPs, MDPs.  

This was the product of my **planned** schedule (ba-dum-psh) rubbing
up against my **actual** schedule. Before the semester started, Anselm
and I worked out a rough schedule for the course, and which classes
I'd be teaching (I specifically wanted to teach CSPs, Bayes Nets, and Approximate
Inference (because I had specific in class exercises in mind), and
Markov Logic and Factored MDPs (because these are fairly new topics I
wanted to season the main course with (more puns! (nested
parentheses!)))).
However, once the semester actually started, several wrenches were
quickly thrown into the mix.

## Best Laid Plans ##

First, I got papers accepted to several
conferences. While this was a good thing for my research progress, it
meant that I would no longer be at Tufts at the time I was supposed to
teach two of my sessions. To avoid changing what sessions I'd be
teaching, we had to get creative with the schedule. This involved many
small schedule shuffles, such as
putting *searching with non-deterministic actions* off for *a month*
in order to shift things back a week.   

Second, to get students ready for the modern AI section, we decided to
combine the lectures on Bayes' Theorem and Utility Theory, and move
them earlier into the course as a sort of "preview for things to come".  

Finally, of course, things just didn't time out exactly as we
expected. Some topics took more time than expected, some took less. In
order to stay on the safe side, advanced planning topics got put off
for a bit, and then, as discussed, ended up getting peppered in
between my other lectures, whose dates were set in stone to accommodate
my conference travels. It was a whirlwind.  

## Conclusions... ##

My first time teaching was certainly a learning experience. If it
weren't for the fact that I was scheduled to teach very specific
sessions of the class, the schedule would certainly have been saner;
presumably it will be *much* saner when I end up teaching the course
by myself at some other university, on my schedule alone.  

Schedule notwithstanding, however, the semester was incredibly
rewarding. I had an absolute blast, and my students seemed to enjoy it
too. I ended up getting an average rating of 4.63 out of 5.0 on my teaching
evaluations, whatever that means, and one student wrote the following,
which made me pretty proud:  

“I have never
had someone put such a visible effort into each lecture and I really
appreciated seeing all the time and hard work Tom put into making sure
we had the best learning experience possible."  

Of course, my students were *significantly* less positive about some
of the homework assignments I designed. But that's a story for another
blog post...
