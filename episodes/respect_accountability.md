---
title: "Respect and Accountability"
teaching: 15 # teaching time in minutes
exercises: 30 # exercise time in minutes
---

:::::::::::::::::::::::::::::::::::::: questions 

- How do you write a lesson using Markdown and `{sandpaper}`?

::::::::::::::::::::::::::::::::::::::::::::::::

::::::::::::::::::::::::::::::::::::: objectives

- Describe key environmental concerns relating to GenAI and machine learning
- State key issues relating to data workers and workers rights
- Awareness of embedded values in the tools
- Describe current legal and ethical debates relating to GenAI

::::::::::::::::::::::::::::::::::::::::::::::::

## Introduction

We have explored a number of dimensions of research integrity through this lesson, including rigour and transparency.

In this episode we will consider the dimensions of respect and accountability.

From the [UK Research Integrity Office on What is Research Integrity](https://ukrio.org/research-integrity/what-is-research-integrity/):

**Care and respect** are expected for everyone and everything involved in the research system, and for the protection of the integrity of the research record. They should be extended to everyone involved in the research process, all participants in research, and for the subjects, users and beneficiaries of research, including humans, animals, the environment and cultural objects. Those engaged with research must also show care and respect for the integrity of the research record.

**Accountability** is expected of everyone individually and collectively to create a research environment in which diverse individuals and organisations are empowered and enabled to own the research process and be accountable for their contributions to the research record. This includes being accountable to participants involved in research, and a responsibility to hold individuals and organisations to account when behaviour falls short of the standards set by the Concordat.

::::::::::::::::::::::::::::::::::::: discussion

## Respect, accountability and GenAI

- Could we fall foul of these obligations through using GenAI?
- What do we need to consider?

We will explore a range of key considerations in this episode.

::::::::::::::::::::::::::::::::::::::::::::::::

## GenAI, machine learning and the environment

Generative AI has a long history although it has only recently gained widespread attention. Building generative AI models involves selecting an appropriate model and algorithm, and training that algorithm on data.

Machine learning, an important subfield of AI, trains algorithms to recognize patterns in data and make predictions or decisions without being explicitly programmed. Computers can learn from experience and improve their performance over time. Machine learning is the foundation of most AI models and tools.

Neither AI nor machine learning are new. Both have been around for decades and both have caused concern about environmental effects of their use during these decades. The key difference between then and now is computing power and scale. Relatively recent advances in computer science have enabled generative AI to become more widespread as mass-market consumer products. Data center buildout has been extremely rapid, increasing the scale in which generative AI is employed. AI data centers require enormous amounts of electricity and water, which strains local resources.

::::::::::::::::::::::::::::::::::::: challenge

Use these resources to help to answer the following questions:

- [What are data centres and how sustainable are they?](https://post.parliament.uk/research-briefings/post-pn-0762/)
- [Critical Minerals in AI and Digital Technologies](https://www.sfa-oxford.com/knowledge-and-insights/critical-minerals-in-low-carbon-and-future-technologies/critical-minerals-in-artificial-intelligence/)
- [I Love Generative AI and Hate the Companies Building It](https://cwodtke.medium.com/i-love-generative-ai-and-hate-the-companies-building-it-3fb120e512ac)

## Question 1: How has genAI availability as a public service changed the scale of environmental impact, even though powerful models already existed long before?

:::::::::::::::::::::::: solution 

A powerful model used by a small number of researchers has a very different environmental footprint than the same (or similar) model fielding requests from millions of users daily. Massive new use of genAI is what transformed environmental impact from a small-scale concern into a broader sustainability question. The scale of public use, not the technology itself, drives the sustainability question.

:::::::::::::::::::::::::::::::::

## Question 2: Describe three kinds of resources that are strained by demand.

:::::::::::::::::::::::: solution 

electricity, hardware/equipment, water

:::::::::::::::::::::::::::::::::

::::::::::::::::::::::::::::::::::::::::::::::::

## Decent work? 

All forms of machine learning require human input. This is either in the form of labelling the training data, or increasingly in reviewing and verifying outputs for model correction and future training.

Issues relating to worker exploitation have been well documented, an example is: 
[My Experience as an Amazon Mechanical Turk (MTurk) Worker](https://www.psychologytoday.com/gb/blog/the-science-behind-behavior/201507/my-experience-as-an-amazon-mechanical-turk-mturk-worker)

Have things gotten better since 2015?

::::::::::::::::::::::::::::::::::::: challenge

## Data workers

Explore [UN SDG 8: Promote sustained, inclusive and sustainable economic growth, full and productive employment and decent work for all](https://sdgs.un.org/goals/goal8)

Watch: [Data Workers Inquiry video](https://youtu.be/tAMqrXlEPDI?si=qesPhySFUOP4Vf30)

Write a minute paper answering the question: Is there a tension between the issues raised by the Data Workers Inquiry and UN SDG 8?


::::::::::::::::::::::::::::::::::::::::::::::::

::::::::::::::::::::::::::::::::::::: instructor

You may choose to explore the UN SDG and watch the video as a group.

Once learners have had an opportunity to reflect and draft the minute paper, you may want to engage them in a discussion around the question:

Have things gotten better since 2015?

::::::::::::::::::::::::::::::::::::::::::::::::




::::::::::::::::::::::::::::::::::::: keypoints 

- Use `.md` files for episodes when you want static content
- Use `.Rmd` files for episodes when you need to generate output
- Run `sandpaper::check_lesson()` to identify any issues with your lesson
- Run `sandpaper::build_lesson()` to preview your lesson locally

::::::::::::::::::::::::::::::::::::::::::::::::

