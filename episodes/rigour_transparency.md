---
title: "Rigour and Transparency"
teaching: 10 # teaching time in minutes
exercises: 2 # exercise time in minutes
---

:::::::::::::::::::::::::::::::::::::: questions 

- How do you write a lesson using Markdown and `{sandpaper}`?

::::::::::::::::::::::::::::::::::::::::::::::::

::::::::::::::::::::::::::::::::::::: objectives

- Awareness of reproducibility concerns re: genAI outputs
- awareness of limitations of explainable AI
- awareness of business models and how these impact behaviours
- describe how genAI use can impact disciplinary norms
- describe reputational impact resulting from lack of transparency around use

::::::::::::::::::::::::::::::::::::::::::::::::

## What is transparency?

The UK Research Integrity Office define Transparency as a means of promoting trust and confidence.

This is demonstrated through:

- reporting full methods,
- publishing all results,
- sharing data, code and materials,
- and declaring conflicts of interest.

This includes acknowledging the use of tools such as emerging technologies, e.g. Generative AI.

::::::::::::::::::::::::::::::::::::: quote

"If you don’t pay for it you are the product"

Margaret McCartney, 2018

::::::::::::::::::::::::::::::::::::::::::::::::

## Open Acccess versus Open Source

There is a wide range of Generative AI and more specifically, Large Language Models that are "free" to use without registering for an account. These often offer very little control over what data is collected during use and re-used for future model training.

Although subscriptions provide a level of control over what data is collected about your use, their is limited information available about how the tool was created. They are often closed source.

How do you know you have used an appropriate method, if you do not know how the tool is deciding what to present to you?

::::::::::::::::::::::::::::::::::::: discussion

### Think, Pair, Share

Read the [definition of open source AI](https://opensource.org/ai/open-source-ai-definition). 

How does the Open Source AI definition compare to the [Open Source definition](https://opensource.org/osd)?

How much does it reduce blackbox and aid explainability?

Spend 2 minutes thinking about your response.

Take it in turns to share your thoughts with your neighbours.

::::::::::::::::::::::::::::::::::::::::::::::::

### Explainable AI

Explainable AI refers to: the set of processes and methods that allows human users to comprehend and trust the results and output created by machine learning algorithms

Is Open Source AI explainable AI?

For more information about explainable AI see: [What is Explainable AI? - Software Engineering Institute, Carnegie Mellon University](https://www.sei.cmu.edu/blog/what-is-explainable-ai/)

## Disciplinary norms and the attention economy

Pre-learning: introduce concept of attention economy, and how this relates to follow-up questions. Relate to pre-registration concept

::::::::::::::::::::::::::::::::::::: challenge 

### Challenge: Task review

Read the aim of the task:

Read the chat transcript:

Answer the questions:

- the prepared plan was adhered to
- if the original objective was met

:::::::::::::::::::::::: solution 



:::::::::::::::::::::::::::::::::

::::::::::::::::::::::::::::::::::::::::::::::::

::::::::::::::::::::::::::::::::::::: keypoints 

- Use `.md` files for episodes when you want static content
- Use `.Rmd` files for episodes when you need to generate output
- Run `sandpaper::check_lesson()` to identify any issues with your lesson
- Run `sandpaper::build_lesson()` to preview your lesson locally

::::::::::::::::::::::::::::::::::::::::::::::::

[r-markdown]: https://rmarkdown.rstudio.com/
