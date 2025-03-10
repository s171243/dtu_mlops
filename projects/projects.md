---
layout: default
title: Projects
nav_order: 12
permalink: projects
---

# Project work
<!-- 
{: .no_toc } 

<details open markdown="block">
  <summary>
    Table of contents
  </summary>
  {: .text-delta }
1. TOC
{:toc}
</details>
-->

---

Approximately 1/3 of the course time is dedicated to doing project work. The projects will serve as the basis of your
exam. In the project, you will essentially re-apply everything that you learn throughout the course to a self chosen project.
The overall goals with the project is:

* To formulate a project within the provided guidelines
* Apply the material though in the course to the problem
* Present your findings

In the projects you are free to work on whatever problem that you want. That said, the only requirement that we have is
that you should incorporate one of the listed below frameworks from the pytorch ecosystem into your project.

## The Pytorch Ecosystem

The [Pytorch ecosystem](https://pytorch.org/ecosystem/) is a great place for finding open-source frameworks
that can help you accelerate your own research. Today we will have focus on three such frameworks from which
you will have to choose one as the foundation for your project. The three frameworks are:

* [Kornia](https://github.com/kornia/kornia). Kornia is a differentiable computer vision (CV) library for PyTorch,
  that consists of a set of routines and differentiable modules to solve generic computer vision problems.
   
* [Transformers](https://github.com/huggingface/transformers). The Transformers repository from the Huggingface group
  focuses on state-of-the-art Natural Language Processing (NLP). It provides many pre-trained model to perform tasks on 
  texts such as classification, information extraction, question answering, summarization, translation, text generation, 
  etc in 100+ languages. Its aim is to make cutting-edge NLP easier to use for everyone.

* [Pytorch-Geometric](https://github.com/rusty1s/pytorch_geometric). PyTorch Geometric (PyG) is a geometric deep learning 
  extension library for PyTorch. It consists of various methods for deep learning on graphs and other irregular structures, 
  also known as geometric deep learning, from a variety of published papers.

Today is also dedicated to doing project work. Remember that the focus of the project work is not
to demonstrate that you can work with the biggest and baddest deep learning model, but instead that you show
that you can incorporate the tools that are taught throughout the course in a meaningful way.

Also note that the project is not expected to be very large in scope. It may simply be that you
want to train X model on Y data. You will approximately be given 4 full days to work on the project.
It is better that you start out with a smaller project and then add along the way if you have time.

### Exercises

1. (Optional) Familiar yourself with each of the libraries. One way to do this is to find relevant tutorials on each project  and try to figure out the code. Such tutorials will give you a rough idea how the API for each library looks like.

2. Form groups! The recommended group size is 4 persons, but we also accept 3 or 5 man groups. Try to other people based
   on what framework that you would like to work with.

3. Brainstorm projects! Try to figure out exactly what you want to work with and especially how you are going to incorporate
   the framework that you have chosen to work with into your project. The **Final exercise** for today is to formulate a
   project description (see bottom of this page).

4. When you formed groups and formulated a project you are allowed to start working on the actual code. I have included a to-do list at the bottom that somewhat summaries what we have done in the course until know. You are **NOT** expected to fulfill all bullet points on the to-do list today, as you will continues to work on the project in the following two weeks. 

### Final objective

Final exercise for today is making a project description. Write around half to one page about:

* Overall goal of the project
* What framework are you going to use (Kornia, Transformer, Pytorch-Geometrics)
* How to you intend to include the framework into your project
* What data are you going to run on (initially, may change)
* What deep learning models do you expect to use

The project description will serve as an guideline for us at the exam that you have somewhat
reached the goals that you set out to do. 

By the end of the day (17:00) you should upload your project description + whatever you have done on the project
until now to github. When this is done one of your group members should send a email to **nsde@dtu.dk** with:

* Link to github page
* The study number of all members of the group
* Your project description

We will briefly look over your github repository and project description to check that everything is fine.

## Project checklist

Please note that all the lists are *exhaustive* meaning that I do not expect you to have completed very
point on the checklist for the exam.

### Week 1

- [ ] Create a git repository
- [ ] Make sure that all team members have write access to the github repository
- [ ] Create a dedicated environment for you project to keep track of your packages
- [ ] Create the initial file structure using cookiecutter
- [ ] Fill out the `make_dataset.py` file such that it downloads whatever data you need and 
- [ ] Add a model file and a training script and get that running
- [ ] When you have something that works somewhat, remember at some point to to some profiling and see if you can optimize your code
- [ ] Remember to fill out the `requirements.txt` file with whatever dependencies that you are using
- [ ] Write unit tests for some part of the codebase and calculate the 
- [ ] Get some continues integration running on the github repository
- [ ] Use either tensorboard or wandb to log training progress and other important metrics/artifacts in your code
- [ ] Remember to comply with good coding practices (`pep8`) while doing the project 

### Week 2

- [ ] Setup and use Azure to train your model
- [ ] Played around with distributed data loading
- [ ] (not curriculum) Reformat your code in the pytorch lightning format
- [ ] Deployed your model using Azure
- [ ] Checked how robust your model is towards data drifting
- [ ] Deployed your model locally using TorchServe

### Week 3

- [ ] Used Optuna to run hyperparameter optimization on your model
- [ ] Wrote one or multiple configurations files for your experiments
- [ ] Used Hydra to load the configurations and manage your hyperparameters

### Additional

- [ ] Revisit your initial project description. Did the project turn out as you wanted?
- [ ] Make sure all group members have a understanding about all parts of the project
- [ ] Created a powerpoint presentation explaining your project
- [ ] Uploaded all your code to github
