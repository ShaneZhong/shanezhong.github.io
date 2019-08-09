---
title: "Sentiment analysis using BERT"
layout: post
date: 2019-04-28 20:19
tag: jekyll
image: https://koppl.in/indigo/assets/images/jekyll-logo-light-solid.png
headerImage: false
projects: true
hidden: true # don't count this post in blog pagination
description: "Sentiment analysis using BERT"
category: project
author: shanezhong
externalLink: false
---

### Summary
If you’ve been following Natural Language Processing over the past year, you’ve probably heard of BERT: 
Bidirectional Encoder Representations from Transformers. It’s a neural network architecture designed 
by Google researchers that’s totally transformed what’s state-of-the-art for NLP tasks, 
like text classification, translation, summarization, and question answering.

Now that BERT's been added to TF Hub as a loadable module, it's easy(ish) to add into existing 
Tensorflow text pipelines. In an existing pipeline, BERT can replace text embedding layers like ELMO 
and GloVE. Alternatively, finetuning BERT can provide both an accuracy boost and faster training time in many cases.

In the Colab below, we'll train a model to predict whether an IMDB movie review is positive 
or negative using BERT in Tensorflow with tf hub.

---
### Colab Code Link
* [Predicting Movie Review Sentiment with BERT on TF Hub](https://colab.research.google.com/drive/1mD-Tt7mpHMoaBEMhgJeEGyXKPmE5eBWZ)
