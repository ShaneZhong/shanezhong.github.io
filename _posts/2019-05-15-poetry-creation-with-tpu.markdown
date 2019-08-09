---
title: "Poetry creation using TPU and GPU"
layout: post
date: 2019-05-15 20:19
tag: jekyll
image: https://koppl.in/indigo/assets/images/jekyll-logo-light-solid.png
headerImage: false
projects: true
hidden: true # don't count this post in blog pagination
description: "Create a 2-layer LSTM model with Chinese poems with Google GPU & TPU "
category: project
author: shanezhong
externalLink: false
---

## Chinese Poetry Creation with TPU and GPU

#### Summary
The aim of this project is to train a 2-layer LSTM neural-network using TPU and GPU on Google
Colab, then compare the training performance of the two approaches.

Long short-term memory (LSTM) is an artificial recurrent neural network (RNN) 
architecture used in the field of deep learning. It is commonly used in building 
Natural-Language-Process (NLP) model and time-series forecast. In this project, the 2-layer LSTM
model contains 73 cells, and each cell contains an embedding layer with 512 dimensions. The
neutral-network layer structure can be summarised as below:
```buildoutcfg
_________________________________________________________________
Layer (type)                 Output Shape              Param #   
=================================================================
seed (InputLayer)            (1024, 73)                0         
_________________________________________________________________
embedding_1 (Embedding)      (1024, 73, 512)           2242048   
_________________________________________________________________
lstm_2 (LSTM)                (1024, 73, 512)           2099200   
_________________________________________________________________
lstm_3 (LSTM)                (1024, 73, 512)           2099200   
_________________________________________________________________
time_distributed (TimeDist)  (1024, 73, 4379)          2246427   
=================================================================
Total params: 8,686,875
Trainable params: 8,686,875
Non-trainable params: 0
_________________________________________________________________
```

The model learns from 20,000 existing Chinese poems to generate a new poem with maximum of 56
characters in 2 sentences. The final output would be similar to the one below:

```
西半登楼送酒船，桐乡方近是羁魂。
海云心事春风恶，长复危亭怨别人。
不及孤城两堪位，即应分别在乡人。
地中宜著金袍玉，更得同盘折角巾。
```


By monitoring the training loss, it is estimated that the model trained on TPU learns 5 times quicker
than the model trained on GPU. You can access both models in the links below.

---
#### Colab Code Link
* [Chinese Poetry Creation with TPU](https://colab.research.google.com/drive/192OqufBtem0KW5geZ3W4oih98ziRnH4M)
* [Chinese Poetry Creation with GPU](https://colab.research.google.com/drive/1hUNOFg29gCuNOoI0uF0kBbWogr3MUIYD)
