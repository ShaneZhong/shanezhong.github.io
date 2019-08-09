---
title: "Regression, Bernoulli Naive Bayes, SVM, XGBoost"
layout: post
date: 2019-04-25 20:19
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
### Kaggle Jupyter Notbook
* Regression, Bernoulli Naive Bayes, SVM, XGBoost and ensemble model to classify customer sentiment - 
[here](https://www.kaggle.com/shaxar/data-science-challenge)

---

### Sentiment Analysis Overview
The focus of this is on a field within machine learning called Natural Language Processing. We can think of this field as the intersection between language, and machine learning. Tasks in this field include automatic translation (Google translate), intelligent personal assistants (Siri), predictive text, and speech recognition for example.

NLP uses many of the same techniques as traditional data science, but also features a number of specialised skills and approaches. There is no expectation that you have any experience with NLP, however, to complete the challenge it will be useful to have the following skills:

understanding of the python programming language, or similar third generation language.
understanding of basic machine learning concepts, i.e. supervised learning


### High-Level Methodology
The following steps are implemented in this notebook to develop a sentiment-detection model:

#### Data Preparation

1. Split the whole dataset into 80% training and 20% testing with stratified sampling
1. Remove special characters, stop words and tokenise the sentences
1. Convert the word tokens into tf-idf matrix format

#### Model Training

1. Train four models: Logistic Regression, Bernoulli Naive Bayes, SVM, XGBoost
1. Apply 10-fold stratified cross-validation to avoid overfitting
1. Apply either Grid Search or Random Search to fine-tune hyperparameters

#### Model Evaluation

1. Plot ROC curves, and calculate AUC-ROC, F1 Score, precision and recall of the four models
1. Plot confusion matrix of the top two models
1. Ensemble the top two models
1. Select the final model based on AUC and F1 score

