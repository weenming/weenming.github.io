---
layout: post
title: "PyTorch Notes"
date: 2023-2-6 +0300
type: "post"
---

Official tutorial [here](https://pytorch.org/tutorials/beginner/basics/data_tutorial.html).
Github repo of my examples [here]()

> While training a model, we typically want to pass samples in “minibatches”, reshuffle the data at every epoch to reduce model overfitting, and use Python’s multiprocessing to speed up data retrieval.
Is it equivalent to randomizing the gradient and is minibatching a common practice in training NNs?
Use DataLoader to load datasets and generate mini-batches