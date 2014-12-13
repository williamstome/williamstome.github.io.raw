---
layout: post
title: "Book and Article Recommendations"
modified: 2014-11-05
excerpt: "From time to time, people ask me for book recommendations pertaining to my research area (Natural Language Dialogue meets Robotics meets Artificial Intelligence)."
tags: [human-robot interaction, natural language, dialog, robotics, books, artificial intelligence]
image:
  feature: features/bookrecs.png
  credit: Azrasta
  creditlink: https://www.flickr.com/photos/azrasta/5088254388/in/photolist-oYHm-aGsP14-51t5TC-8KCCKW-4hn47g-7PozJp-mBGj-84P71r-7HoeXV-UmBz-5NZzVJ-dphot9-ntNE-6DfhNt-ahytco-ca5ZF-9kHQKs-ix8Rbz-cBJ5d-eqHuv-6NP8d6-aT9to6-9K3BPW-2PgAx-97oiDM-aRxNm-fo562E-HdurS-aibaen-7Nbvbk-KLWAb-maAU6-amWKZg-6buevW-6GjMcy-amWKX6-amWKYM-7acJMF-8DFBf3-MLnGM-9TvtEQ-abK4Bq-dGa2xi-2U9nA-bF4Yf7-6Knypk-hss2M-61kymQ-f4HeM7-9ZVvhF
date: 2014-10-20
comments: true
---

From time to time, people ask me for book recommendations pertaining
to my research area (Natural Language Dialogue meets Robotics meets
Artificial Intelligence). Unfortunately, I rarely have a satisfying
answer to this question, as I don't actually know of any books that
sit at this precise intersection of fields. Everything I know about my
research area I learned by reading conference papers and journal
articles; if there are books on the topic, I'd love to read them, and
I should be reading them, but unfortunately I'm just not aware of the
existence of any such books.

What I *can* do is recommend (1) survey articles on closely related
topics, and (2) books on more tangentially related topics. Here we go!

# Survey Articles

## Human-Robot Interaction

I work in the Human-Robot Interaction Lab. What the heck is
Human-Robot Interaction? If you're interested in this question, I'd
read 
[Socially intelligent robots: dimensions of human–robot interaction](http://www.ncbi.nlm.nih.gov/pmc/articles/PMC2346526/)
by Kerstin Dautenhahn. This article gives a great
overview of HRI, why it's important, and what typifies an HRI
Experiment.

> Social intelligence in robots has a quite recent history in artificial
> intelligence and robotics. However, it has become increasingly
> apparent that social and interactive skills are necessary requirements
> in many application areas and contexts where robots need to interact
> and collaborate with other robots or humans. Research on human–robot
> interaction (HRI) poses many challenges regarding the nature of
> interactivity and ‘social behaviour’ in robot and humans. The first
> part of this paper addresses dimensions of HRI, discussing
> requirements on social skills for robots and introducing the
> conceptual space of HRI studies. In order to illustrate these
> concepts, two examples of HRI research are presented. First, research
> is surveyed which investigates the development of a cognitive robot
> companion. The aim of this work is to develop social rules for robot
> behaviour (a ‘robotiquette’) that is comfortable and acceptable to
> humans. Second, robots are discussed as possible educational or
> therapeutic toys for children with autism. The concept of interactive
> emergence in human–child interactions is highlighted. Different types
> of play among children are discussed in the light of their potential
> investigation in human–robot experiments. The paper concludes by
> examining different paradigms regarding ‘social relationships’ of
> robots and people interacting with them. 

## DIARC

While the previous article gives a great explanation of the field
of HRI, it mainly focuses on human-subject experiments; in the HRI
Lab, this is only one branch of our research. The other main branch
of our research is on the development of AI Algorithms to
*facilitate* the goals of HRI, i.e., natural human-robot
interaction. For an overview of the algorithm development that goes
on in our lab, I'd read
[Novel mechanisms for natural human-robot interactions in the DIARC architecture](http://hrilab.tufts.edu/publications/aaai13irsfinal.pdf) by Scheutz et al. (Disclaimer: I'm one of the al.'s
you can call me Al.) 

> Natural human-like human-robot interactions require many
> functional capabilities from a robot that have to be reflected in
> architectural components in the robotic control architecture.
> In particular, various mechanisms for producing social behaviors,
> goal-oriented cognition, and robust intelligence are 
> required. In this paper, we present an overview of the most recent
> version of our DIARC architecture and show how several 
> novel algorithms attempt to address these three areas, leading
> to more natural interactions with humans, while also extending the
> overall capability of the integrated system. 

## Natural-Language Dialogue

For a more targeted overview of the types of problems I'm
interested in, I'd read the following three papers:

### Statistical Techniques for Natural Language Processing

[Statistical Techniques for Natural Language Processing](http://cs.brown.edu/~ec/papers/aimag97.ps) by Eugene
Charniak: this paper is almost two decades old, but it gives an
easy-to-parse (pun!) overview of the main problems in NLP.

> We review current statistical work on syntactic parsing and then
> consider part-of-speech tagging, which was the first syntactic problem
> to be successfully attacked by statistical techniques and also serves
> as a good warmup for the main topic, statistical parsing. Here we
> consider both the simplified case in which the input string is viewed
> as a string of parts of speech, and the more interesting case in which
> the parser is guided by statistical information about the particular
> words in the sentence. Finally we anticipate future research
> directions.  

### Challenges for Spoken Dialogue Systems

[Challenges for Spoken Dialogue Systems](https://www.google.com/url?sa=t&rct=j&q=&esrc=s&source=web&cd=2&cad=rja&uact=8&ved=0CCkQFjAB&url=http%3A%2F%2Fwww.cs.cmu.edu%2F~.%2Fdgroup%2Fpapers%2Fglass99.pdf&ei=-81FVN6YF4rbsATWo4H4Bw&usg=AFQjCNHrs-HBonhcvyuixsEWynHb5TyGng&sig2=or7pnICUE3G_lNA3iDMnNQ&bvm=bv.77880786,d.cWc) by James R. Glass: this paper
is almost as old, but it paints a good picture of 
where the problems from the previous paper sit in relation to the
other problems in dialogue processing.

> The past decade has seen the development of a large number of spoken
> dialogue systems around the world, both as research prototypes and
> commercial applications. These systems allow users to interact with a
> machine to retrieve information, conduct transactions, or perform
> other problem-solving tasks. In this paper we discuss some of the
> design issues which confront developers of spoken dialogue systems,
> provide some examples of research being undertaken in this area, and
> describe some of the ongoing challenges facing current spoken language
> technology. 

### Recent Approaches to Dialog Management for Spoken Dialog Systems

[Recent Approaches to Dialog Management for Spoken Dialog Systems](http://jcse.kiise.org/posting/4-1/jcse_4-1_56.pdf) by Cheongjae Lee et al.:
this paper is much newer, and shows how the field of Natural
Language Dialogue has evolved since the Glass paper was
published. Some of the same problems are waiting to be solved,
and other problems are brand new. 

> A field of spoken dialog systems is a rapidly growing research area because the performance
> improvement of speech technologies motivates the possibility of building systems that a human
> can easily operate in order to access useful information via spoken languages. Among the
> components in a spoken dialog system, the dialog management plays major roles such as
> discourse analysis, database access, error handling, and system action prediction. This survey
> covers design issues and recent approaches to the dialog management techniques for modeling
> the dialogs. We also explain the user simulation techniques for automatic evaluation of spoken
> dialog systems.

# Books

The four books I'd recommend are much broader in scope. 

## Godel, Escher, Bach

First, I'd recommend [Godel, Escher, Bach](http://www.amazon.com/G%C3%B6del-Escher-Bach-Eternal-Golden/dp/0465026567/ref=sr_1_1?ie=UTF8&qid=1413861409&sr=8-1&keywords=godel+escher+bach) by Douglas
R. Hofstadter. This is the book that 
got me hooked on A.I. and Cognitive Science. I am by no means unique
in this position; at one point, there were four different copies of
this book in my lab. As the title suggests, Hofstadter ties together
elements of the number theory of Godel, the art of Escher, and the
music of Bach. Parts of the book are pure fun (e.g., cyclic
engravings by Escher, followed by music by Bach that reads the same
backwards and forwards, followed by a dialogue that reads the same
backwards and forwards), and parts of it are pretty dense number
theory. It's almost 800 pages but I've read it twice and
periodically revisit particularly entertaining sections. It's a
masterpiece that will inspire you to think about AI, and it's only
$15 on Amazon. Go buy it now.

## Robot Ethics

For something a little more robot oriented, I'd recommend
[Robot Ethics](http://www.amazon.com/Robot-Ethics-Implications-Intelligent-Autonomous/dp/026252600X/ref=sr_1_1?ie=UTF8&qid=1413861857&sr=8-1&keywords=robot+ethics), a collection of essays by robo-ethicists. Some essays
are certainly better than others (subjective opinion), and I'm
still working my way through it, but it will certainly change the
way you think about robot warriors and sexbots, both of which
present a whole host of interesting ethical questions, and, oh,
both of which are *already here*. This book is $20 on Amazon.

## The Cambridge Handbook of Computational Psychology

Okay. This one's a bit of a
sell. [The Cambridge Handbook of Computational Psychology](http://www.amazon.com/Cambridge-Handbook-Computational-Psychology-Handbooks/dp/0521674107/ref=sr_1_1?ie=UTF8&qid=1413862097&sr=8-1&keywords=cambridge+handbook+computational+psychology) (ed. Ron
Sun) It's $70 on Amazon ($45 
used). That being said, you can find various chapters from it
around the internet. This is a collection of survey articles on
various cognitive modeling topics. The first few chapters of the
book are on modeling paradigms (Connectionist, Bayesian, Dynamical
Systems, Logical, Production Systems) by some of the biggest names
in the respective areas. The rest of the book describes computational
models of various mental processes: episodic memory,
categorization, decision making, psycholinguistics, scientific
explanation, etc. It's an invaluable resource for someone
interested in cognitive science (well, it's a $70 resource).

## Natural Language Understanding and Pragmatics ##

If you're interested in learning about my specific research area, I'd
recommend Georgia M. Green's [Natural Language Understanding and
Pragmatics](http://www.amazon.com/Pragmatics-Language-Understanding-Tutorial-Cognitive/dp/080582166X),
for so many reasons. This little book is only around 150 pages, and
will cost you around $20 on Amazon. Now that might sound like a high
cost-per-page ratio but I really can't reccommend this book strongly
enough. It's an accessible, informative, concise, and well-organized
introduction to the various topics of import to my main field of
study: pragmatic analysis. While it contains no algorithms or even
much in the way of discussion thereof, this is an incredibly useful
little book that has gotten me excited with lots of new ideas, despite
the fact that it's 20 years old. I would recommend it to both
academics and lay persons alike: it's short, it's sweet, it's
fascinating.  

# Conclusions
Those are my suggestions! I would love to hear others' suggestions for
accessible but substantial material in related fields.