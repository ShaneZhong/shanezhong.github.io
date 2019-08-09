---
title: "Twitter bot with GPT-2"
layout: post
date: 2019-08-09 22:10
tag: jekyll
image: https://koppl.in/indigo/assets/images/jekyll-logo-light-solid.png
headerImage: false
projects: true
hidden: true # don't count this post in blog pagination
description: "This is a simple and minimalist template for Jekyll for those who likes to eat noodles."
category: project
author: shanezhong
externalLink: false
---

#### AI Generated tweet using GPT-2 model
* The twitter account link [here](https://twitter.com/ai_telling)

* To set up the email notification - please visit [here](https://support.google.com/mail/answer/7126229?visit_id=636997950280030700-282303594&rd=2#cantsignin)

* Github link - [here](https://github.com/ShaneZhong/gpt-2-twitter-bot)

---
#### gpt-2

Code from the paper ["Language Models are Unsupervised Multitask Learners"](https://d4mucfpksywv.cloudfront.net/better-language-models/language-models.pdf).

We have currently released small (117M parameter) and medium (345M parameter) versions of GPT-2.  While we have not released the larger models, we have [released a dataset](https://github.com/openai/gpt-2-output-dataset) for researchers to study their behaviors.

See more details in our [blog post](https://blog.openai.com/better-language-models/).

#### Usage

This repository is meant to be a starting point for researchers and engineers to experiment with GPT-2.

#### Some caveats

- GPT-2 models' robustness and worst case behaviors are not well-understood.  As with any machine-learned model, carefully evaluate GPT-2 for your use case, especially if used without fine-tuning or in safety-critical applications where reliability is important.
- The dataset our GPT-2 models were trained on contains many texts with [biases](https://twitter.com/TomerUllman/status/1101485289720242177) and factual inaccuracies, and thus GPT-2 models are likely to be biased and inaccurate as well.
- To avoid having samples mistaken as human-written, we recommend clearly labeling samples as synthetic before wide dissemination.  Our models are often incoherent or inaccurate in subtle ways, which takes more than a quick read for a human to notice.
