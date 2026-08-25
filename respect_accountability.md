---
title: "Respect and Accountability"
teaching: 30 # teaching time in minutes
exercises: 30 # exercise time in minutes
---

:::::::::::::::::::::::::::::::::::::: questions 

- Why is there concern about the environmental impacts of GenAI?
- What is a data worker?
- What influences the output from a GenAI tool?
- What are the IP and data protection considerations when using GenAI tools?

::::::::::::::::::::::::::::::::::::::::::::::::

::::::::::::::::::::::::::::::::::::: objectives

- Describe key environmental concerns relating to GenAI and machine learning
- State key issues relating to data workers and worker rights
- Describe embedded values in the tools
- Describe current legal and ethical debates relating to GenAI

::::::::::::::::::::::::::::::::::::::::::::::::

## Introduction

We have explored a number of dimensions of research integrity through this lesson, including rigour and transparency.

In this episode we will consider the dimensions of respect and accountability.

From the [UK Research Integrity Office on What is Research Integrity](https://ukrio.org/research-integrity/what-is-research-integrity/):

**Care and respect** are expected for everyone and everything involved in the research system, and for the protection of the integrity of the research record. They should be extended to everyone involved in the research process, all participants in research, and for the subjects, users and beneficiaries of research, including humans, animals, the environment and cultural objects. Those engaged with research must also show care and respect for the integrity of the research record.

**Accountability** is expected of everyone individually and collectively to create a research environment in which diverse individuals and organisations are empowered and enabled to own the research process and be accountable for their contributions to the research record. This includes being accountable to participants involved in research, and a responsibility to hold individuals and organisations to account when behaviour falls short of the standards set by the Concordat.

::::::::::::::::::::::::::::::::::::: discussion

### Respect, accountability and GenAI

- Could we fall afoul of these obligations through using GenAI?
- What do we need to consider?

We will explore a range of key considerations in this episode.

::::::::::::::::::::::::::::::::::::::::::::::::

## GenAI, machine learning and the environment

Generative AI has a long history although it has only recently gained widespread attention. Building generative AI models involves selecting an appropriate model and algorithm, and training that algorithm on data.

Machine learning, an important subfield of AI, trains algorithms to recognize patterns in data and make predictions or decisions without being explicitly programmed. Computers can learn from experience and improve their performance over time. Machine learning is the foundation of most AI models and tools.

Neither AI nor machine learning are new. Both have been around for decades and both have caused concern about environmental effects of their use during these decades. The key difference between then and now is computing power and scale. Relatively recent advances in computer science have enabled generative AI to become more widespread as mass-market consumer products. [Data center buildout has been extremely rapid](https://brockovichdatacenter.com/#map-section), increasing the scale in which generative AI is employed. AI data centers require enormous amounts of electricity, water, and land, which strains local resources.

::::::::::::::::::::::::::::::::::::: challenge

Use these resources to help to answer the following questions:

- [What are data centres and how sustainable are they?](https://post.parliament.uk/research-briefings/post-pn-0762/)
- [Critical Minerals in AI and Digital Technologies](https://www.sfa-oxford.com/knowledge-and-insights/critical-minerals-in-low-carbon-and-future-technologies/critical-minerals-in-artificial-intelligence/)
- [I Love Generative AI and Hate the Companies Building It](https://cwodtke.medium.com/i-love-generative-ai-and-hate-the-companies-building-it-3fb120e512ac)

### Question 1: How has genAI availability as a public service changed the scale of environmental impact, even though powerful models already existed long before?

:::::::::::::::::::::::: solution 

A powerful model used by a small number of researchers has a very different environmental footprint than the same (or similar) model fielding requests from millions of users daily. Massive new use of genAI is what transformed environmental impact from a small-scale concern into a broader sustainability question. The scale of public use, not the technology itself, drives the sustainability question.

:::::::::::::::::::::::::::::::::

### Question 2: Describe three kinds of resources that are strained by demand.

:::::::::::::::::::::::: solution 

electricity, land, water

:::::::::::::::::::::::::::::::::

::::::::::::::::::::::::::::::::::::::::::::::::

## Decent work? 

All forms of machine learning require human input. This is either in the form of labelling the training data, or increasingly in reviewing and verifying outputs for model correction and future training.

Issues relating to worker exploitation have been well documented, an example is: 
[My Experience as an Amazon Mechanical Turk (MTurk) Worker](https://www.psychologytoday.com/gb/blog/the-science-behind-behavior/201507/my-experience-as-an-amazon-mechanical-turk-mturk-worker)

Have things gotten better since 2015?

::::::::::::::::::::::::::::::::::::: challenge

## Data workers

Explore [UN Sustainable Development Goal 8: Promote sustained, inclusive and sustainable economic growth, full and productive employment and decent work for all](https://sdgs.un.org/goals/goal8)

Watch: [Data Workers Inquiry video](https://youtu.be/tAMqrXlEPDI?si=qesPhySFUOP4Vf30)

Write a minute paper answering the question: Is there a tension between the issues raised by the Data Workers Inquiry and UN SDG 8?


::::::::::::::::::::::::::::::::::::::::::::::::

::::::::::::::::::::::::::::::::::::: instructor

You may choose to explore the UN SDG and watch the video as a group.

Once learners have had an opportunity to reflect and draft the minute paper, you may want to engage them in a discussion around the question:

Have things gotten better since 2015?

::::::::::::::::::::::::::::::::::::::::::::::::

## The process of model training

LLM models predict tokens. After receiving an input text, also called 'prompt', it essentially predicts the most likely word to follow that text and continues like that up to a certain length.

For example, if you enter the text below in to an LLM, the model continues your text predicting word after word with the Python code:

```{python}
def convert_miles_to_km(
```

LLMs develop the models that allow them to predict the next word by identifying patterns in unimaginably large quantities of text. That process is called pre-training.

These pre-trained models come with a series of flaws. They do not necessarily interpret user input as an instruction or question, so the can be more difficult to use. They also are more likely to produce harmful or false outputs.

To mitigate this, pre-training is usually followed by fine tuning. This process modifies pre-trained models, improves the types of outputs they are likely to produce, and lowers the risk of harmful or wrong output.

There are several fine tuning techniques. One is called reinforcement learning, which aims to maximize a chosen measure of task performance (referred to as a reward signal).

Reinforcement learning requires special machine learning models, called reward models, to provide a reward signal. The reward models take in some text and estimate its quality, usually by providing a numerical score. The score then can serve as the reward signal.

There are two common methods to train reward models.

**Reinforcement Learning From Human Feedback (RLHF)**: Human annotators compare two different model-generated responses to a prompt and choose which is better (example https://arxiv.org/abs/2203.02155)

**Reinforcement Learning From AI Feedback (RLAIF)**: Instead of human annotators an LLM is used to rank the responses. Just like human annotators, the LLM is provided with written instructions on how to rate outputs. (example https://arxiv.org/abs/2212.08073)

It is important to note that fine-tuning does not guarantee that a LLM works perfectly - its just is an improvement over the pre-trained model to reduce risks and make it more user friendly.

::::::::::::::::::::::::::::::::::::: challenge

Given what you have learned about the process of model training, explore with your neighbour: 

What are possible ways for biased views and value judgements to affect the model algorithm?

::::::::::::::::::::::::::::::::::::::::::::::::

## Embedded values

The widespread deployment of LLMs has brought to light many concerns
about biases embedded within the models. There are several ways how biases can enter into the LLMs we use. Below are a few examples.

### Bias in training data

The training data collected from the internet reflect societal biases present in online content, such as gender or racial stereotypes. Similarly, decisions made about which data to collect and how to curate the data, can introduce bias for example by introducing the the over- or under-representation of certain sources.

### Bias in reward model / fine tuning

Human feedback in RLHF trained reward models are based on real human judgments which are inevitably shaped by cognitive biases.

RLAIF trained models are generated using prompts with a set of principles
like “choose the less harmful response,” and asked to judge pairs of outputs.

Both RLHF or RLAIF trained reward models can exhibit so called length bias, a tendency to favor longer responses by conflating verbosity with quality. The reward model correlates response length with quality (longer = more helpful)

### Bias in design decisions

Decisions about the model architecture during model development can impact how biases are represented and amplified. Like all of us, developers have implicit biases, so they may unconsciously make choices that exacerbate existing inequalities or fail to recognize certain biases.

Some architectures may be more prone to certain types of biases due to their structural characteristics or the way they process input data. For example, a model optimized for accuracy might perform better on majority groups while neglecting minority groups.

## Open and Closed Source Models

There are three main levels of model 'openness'.

- Fully open-source models with unrestricted access to code, weights, documentation and training data. Example https://www.apertus-ai.org/
- Models with publicly available weights, which allow for fine-tuning and adaptation but do not disclose training processes or datasets. Example: Mistral and Llama
- Fully closed, proprietary models typically accessible only through APIs or enterprise licenses. Example: GPT-models, Claude, Gemini.

Unfortunately end users are left to deal with these embedded values. Even for fully open source models scrutinizing and adjusting the algorithms is not feasible, unless you are a developer.

::::::::::::::::::::::::::::::::::::: instructor

The following topics currently use legal examples from the UK and Europe. We hope to expand examples from other areas over time.

Please adjust to add examples from your own context.

::::::::::::::::::::::::::::::::::::::::::::::::

## Training data acquisition, was it fair?

Let's revisit care and respect.

Care and respect are expected for everyone and everything involved in the research system, and for the protection of the integrity of the research record.

There are concerns about how the training data was collected for Generative AI tools, and there have been a number of court cases where creators believe their rights have been infringed:

- [Three key AI and copyright cases](https://www.publishers.org.uk/three-key-ai-and-copyright-cases/)
- [The Higher Regional Court of Munich considered memorization and temporary copies occurred in model training as infringing reproductions of works](https://www.euipo.europa.eu/en/law/recent-case-law/the-higher-regional-court-of-munich-considered-memorization-and-temporary-copies-occurred-in-model-training-as-infringing-reproductions-of-works)

::::::::::::::::::::::::::::::::::::: discussion

### Stack Overflow and ChatGPT

Read: [Stack Overflow users sabotage their posts after OpenAI deal](https://arstechnica.com/information-technology/2024/05/stack-overflow-users-sabotage-their-posts-after-openai-deal/)

- Are the contributors to StackOverflow being respected, why and why not?
- Does training a commercial product count as scientific research?

::::::::::::::::::::::::::::::::::::::::::::::::

::::::::::::::::::::::::::::::::::::: callout 

[Using CC-licensed Works for AI Training](https://creativecommons.org/wp-content/uploads/2025/05/Using-CC-licensed-Works-for-AI-Training.pdf)

The Creative Commons guidance notes that differences in national laws around copyright impact on the use of copyrighted materials in training data, it also notes that it may not be possible to attribute materials other than RAG trained systems.

::::::::::::::::::::::::::::::::::::::::::::::::

## Generated outputs and copyright infringements

It is important to check that the outputs of a Generative AI tool is not infringing Copyright.

Currently in the UK:

"Where an AI model is used to generate material that reproduces all or a substantial part of a copyright work without permission this may also comprise an infringement of copyright if there is no relevant exception and no licence is in place. This act of infringement occurs at the output stage and may also create infringement through any subsequent dealing. Any action would be taken against the persons responsible for these respective acts, and depending on the circumstances, the user, the provider of the AI system and any person dealing with infringing content after it has been created may all be liable. Enforcement action against such infringement is available as for other infringements of copyright and would usually be pursued by the right holder through the civil courts."

Source:[UK Government: Report on Copyright and Artificial Intelligence](https://www.gov.uk/government/publications/report-and-impact-assessment-on-copyright-and-artificial-intelligence/report-on-copyright-and-artificial-intelligence)

There have been a number of cases where a generative AI tool has either reproduced or been suspected of reproducing copyrighted materials:

- [Unity promises strong AI copyright 'guardrails' after employee conjures Mickey Mouse on stream](https://www.gamedeveloper.com/art/unity-promises-stronger-ai-copyright-guardrails-after-employee-conjures-mickey-mouse-on-stream)

## Protecting AI generated outputs

In UK law there are existing protections for Computer Generated Works, however, this is not the case in other countries.
[Section I of the UK Government Report on Copyright and Artificial Intelligence](https://www.gov.uk/government/publications/report-and-impact-assessment-on-copyright-and-artificial-intelligence/report-on-copyright-and-artificial-intelligence#section-i-computer-generated-works) outlines differences between UK law and other jurisdictions. 

[The EU report Generative AI and Copyright states](https://www.europarl.europa.eu/RegData/etudes/STUD/2025/774095/IUST_STU(2025)774095_EN.pdf): 

"purely AI-generated outputs—those created automatically by an
AI system without substantial human intervention—are not eligible for copyright protection in the EU.
Such outputs are considered to fall into the public domain, making them freely available for anyone to
use, reproduce, or adapt without seeking permission or providing attribution. " 

::::::::::::::::::::::::::::::::::::: discussion

### Implications for International Collaboration and Publication

It is increasingly common that we are collaborating with colleagues in other institutions, and in other countries.

- Given differences in the ability to protect AI generated outputs, are their any implications for collaborations?
- Could these differences cause problems when publishing research software?

A prompt is insufficient to count as original human work, when is the threshold crossed?

::::::::::::::::::::::::::::::::::::::::::::::::

## Protecting other peoples' data

We often work with varying types of data files. These may contain various qualitative and quantitative data.

If data files are uploaded to or accessed within an AI enabled environment it is not always clear what these tools are able to read, or where they be storing any uploaded data files.

In the UK, the [Data (Use and Access) Act 2025](https://www.legislation.gov.uk/ukpga/2025/18/contents) got Royal Assent on 19 June 2025, as a result there have been a number of updates to Information Commissioner's Office (ICO) guidance. The ICO states that "the use of AI will involve a type of processing likely to result in a high risk to individuals’ rights and freedoms, and will therefore trigger the legal requirement for you to undertake a DPIA."

See: [Guidance on AI and data protection](https://ico.org.uk/for-organisations/uk-gdpr-guidance-and-resources/artificial-intelligence/guidance-on-ai-and-data-protection/what-are-the-accountability-and-governance-implications-of-ai/#DPIA)

Data Privacy Impact Assessments (DPIAs) are a requirement of the General Data Protection Regulation (GDPR), it is recognised by the European Parliament that there is some overlap between the AI Act and GDPR ([Interplay between the AI Act and the EU digital legislative framework](https://www.europarl.europa.eu/thinktank/en/document/ECTI_ATA(2025)778577)). The AI Act also requires the completion of a fundamental rights impact assessment when an AI system is deemed high risk. There are eight areas that are considered high risk ([Annex III: High-Risk AI Systems Referred to in Article 6(2)](https://artificialintelligenceact.eu/annex/3/)), in addition to AI systems that are intended to be used as a safety component of a product.

It is therefore important for us to know what the tools and platforms we are using have access to, and what is being shared. If you are working with commercially sensitive, personal and especially special category data you will want to ensure that you are working in a closed environment that is not transferring data outside of your organisation.

::::::::::::::::::::::::::::::::::::: keypoints 

- The current AI boom is resulting in the building of new large scale data centres.
- New large scale data centres are increasing the demands on energy and water supplies.
- Machine learning relies on human workers, there is a history of poor working practices and lack of support for data workers.
- There is a complex landscape around data protection and copyright, you will need to be aware of both your local regulations and those of any international partners you may have.

::::::::::::::::::::::::::::::::::::::::::::::::

