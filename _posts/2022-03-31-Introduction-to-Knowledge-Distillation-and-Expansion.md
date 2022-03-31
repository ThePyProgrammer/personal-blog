---
toc: false
layout: post
description: Algorithms to bring School to your Model Training Process
categories: [ai]
title: A Brief Introduction to Knowledge Distillation (and Expansion)
---

Knowledge Distillation<sup>[<a href="#ref1">1</a>]</sup> refers to the process where a larger, difficult to deploy model transfers its learned knowledge about its task to a smaller, faster model. This is typically used to reduce large sized models into computationally less expensive models for real-world deployment. The larger model is often termed the "teacher" model, and the smaller model the "student".

Existing work done in the field of knowledge distillation for NLP is limited and focuses on feature-basead knowledge, wherein the student model tries to replicate the feature embeddings (intermediate layers) of the teacher model. This includes work done by Shin et al.<sup>[<a href="#ref2">2</a>]</sup> wherein they use knowledge distillation and ensemble methods for word embedding distillation, as well as Jiang et al.<sup>[<a href="#ref3">3</a>]</sup> that demonstrates knowledge distillation from pretrained BERT models achieves improvements in performance.

### References
<div id="#ref1" />
[1] Geoffrey Hinton, Oriol Vinyals, and Jeff Dean. Distilling the Knowledge in a Neural Network. 2015. DOI: [`10.48550/ARXIV.1503.02531`](https://doi.org/10.48550/ARXIV.1503.02531). URL: [`https://arxiv.org/abs/1503.02531`](https://arxiv.org/abs/1503.02531).
<div id="#href2" />
[2] Bonggun Shin, Hao Yang, and Jinho D. Choi. “The Pupil Has Become the Master: Teacher-Student Model-Based Word Embedding Distillation with Ensemble Learning”. In: Proceedings of the Twenty-Eighth International Joint Conference on Artificial Intelligence, IJCAI-19. International Joint Conferences on Artificial Intelligence Organization, July 2019, pp. 3439–3445. DOI: [`10.24963/ijcai.2019/477`](https://doi.org/10.24963/ijcai.2019/477). URL: [`https://doi.org/10.24963/ijcai.2019/477`](https://doi.org/10.24963/ijcai.2019/477).
<div id="#ref3" />
[3] Yidi Jiang et al. Knowledge Distillation from BERT Transformer to Speech Transformer for Intent Classification. 2021. DOI: [`10.48550/ARXIV.2108.02598`](https://doi.org/10.48550/ARXIV.2108.02598). URL: [`https://arxiv.org/abs/2108.02598`](https://arxiv.org/abs/2108.02598).