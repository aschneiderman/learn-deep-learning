---
layout: content
title: 'Training A Model: Overview'
image: 'colorful-art-supplies-1445895-pxh.jpg'
---

## Basic Overview

Learner: in fastai, used to train a model
Or: a learner is something that can learn to fit a model

Most basic learner, used by intro example of cats and dogs species:
```
learn = create_cnn(data, models.resnet34, metrics=error_rate)
learn.fit_one_cycle(4)		# Training for 5 epochs (5 cycles through the data)
```

- data: data
- arch: your architecture, in this case, ResNet34

Architectures:

- ResNet34 contains pre-trained weights, which effectively means that the model has already been trained for a particular task.
- Why do you have different types of architectures -- e.g., if you want to create a model that's going to run on a smart phone.
- The advantage of ResNet34 is that it works pretty well across a pretty broad range of problems -- and that's part of their general philosophy: "one of the things we try to show you is stuff which just tends to always work even if you don't quite tune everything perfectly" (Lesson 1)


Learn.fit_one_cycle: fitting the model using "one cycle learning"



