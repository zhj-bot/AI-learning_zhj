# Phase 0 Lesson 3 Summary: GPU Setup & Cloud

## What This Lesson Was About

This lesson introduced when AI engineers need GPUs, when ordinary computers are
enough, and why beginners usually should not buy expensive hardware too early.

The main takeaway:

```text
You do not need your own GPU to start learning AI engineering.
```

## Key Concepts

### CPU

CPU means Central Processing Unit. In Chinese, it is usually called the central
processor.

Beginner-friendly meaning:

```text
The CPU is the general-purpose brain of the computer.
```

It handles many normal computer tasks, such as:

- Opening software.
- Running Python scripts.
- Managing files.
- Browsing the web.
- Sending requests to an API.

Simple analogy:

```text
A CPU is like one skilled worker who can handle many different kinds of tasks.
```

### GPU

GPU means Graphics Processing Unit. In Chinese, it is usually called the
graphics processor.

Beginner-friendly meaning:

```text
The GPU is a processor that is very good at doing many similar calculations at
the same time.
```

It was originally designed for graphics and games, but it is also useful for AI
because deep learning often involves a huge number of repeated calculations.

Simple analogy:

```text
A GPU is like a large team of workers doing many small similar jobs in
parallel.
```

### Why AI Uses GPUs

Deep learning models often work with many numbers arranged in tables. These are
called matrices.

Beginner-friendly meaning:

```text
A matrix is a table of numbers.
```

Training a model means repeatedly calculating and adjusting many numbers. GPU
parallel computing can make this much faster.

### API

API means Application Programming Interface.

Beginner-friendly meaning:

```text
An API is a way for your code to use a service provided by someone else.
```

When using the OpenAI API, the model runs on OpenAI's servers. Your computer
sends a request and receives an answer.

Important idea:

```text
Calling an LLM API does not require your own GPU.
```

### Local GPU

A local GPU is a graphics card installed in your own computer.

Pros:

- Can be useful for long-term heavy experiments.
- Data can stay on your own machine.
- No hourly rental fee.

Cons:

- Expensive upfront.
- Environment setup can be difficult.
- Memory may still be too small for large models.

### Cloud GPU

A cloud GPU is a GPU rented from an online platform.

Pros:

- No need to buy hardware.
- Can rent stronger machines only when needed.
- Better for short experiments and learning.

Cons:

- Usually charged by time.
- Forgetting to stop the machine can waste money.
- Data may need to be uploaded.
- Platform setup and billing rules must be understood.

Important rule:

```text
When using a cloud GPU, stop or terminate it as soon as the experiment is done.
```

## Practical Rule for Current Learning Stage

For the current beginner stage:

```text
Python basics: no GPU needed
Git practice: no GPU needed
OpenAI API calls: no personal GPU needed
RAG basics: usually no GPU needed
Deep learning model training: may need GPU
LLM fine-tuning: usually needs GPU
```

Recommended order:

```text
1. Use the local computer CPU first.
2. Try free options such as Colab or Kaggle when training is needed.
3. Rent cloud GPU only when free options are not enough.
4. Consider buying a local GPU only after real repeated need appears.
```

## Exercise Answers and Feedback

### Exercise 1

Question: Which scenarios need GPU?

Your answers:

```text
A. Python basics: no GPU needed
B. OpenAI API: no personal GPU needed
C. Image classification training: may need GPU
D. Git notes: no GPU needed
E. Fine-tuning an open-source LLM: needs GPU
```

Feedback:

All correct. You correctly understood the difference between calling an API and
running/training models yourself.

### Exercise 2

Question 1: Why does calling the OpenAI API not require your own GPU?

Your answer:

```text
Because it runs on the provider's server.
```

Feedback:

Correct. More specifically, the model runs on OpenAI's servers and GPUs. Your
computer only sends the request and receives the result.

Question 2: Why should beginners not buy a GPU immediately?

Your answer:

```text
Because I am still learning the basics and have not reached deep learning model
training yet.
```

Feedback:

Correct. Buying hardware too early can waste money and attention.

Question 3: What is the biggest risk of cloud GPU?

Your answer:

```text
Forgetting the account password and forgetting to turn off the machine, wasting
money.
```

Feedback:

Forgetting the password is inconvenient, but the main cloud GPU risk is
forgetting to stop the machine, which causes ongoing billing.

### Exercise 3

Your answers:

```text
A. Buying a high-end GPU at the start: unreasonable
B. Using an ordinary computer for OpenAI API practice: reasonable
C. Leaving cloud GPU running after experiments: unreasonable
D. Trying Colab or Kaggle before paid GPU: reasonable
```

Feedback:

All correct.

## Learning Preference Added

Important teaching preference:

```text
When a new technical term or concept appears, explain it clearly for a
zero-basis learner before using it in exercises.
```

The explanation should include:

- A plain-language definition.
- A simple analogy.
- Why it matters in AI engineering.
- A small example.

## Learning Progress

Current status:

```text
Phase 0 Lesson 3: completed
```

Understood well:

- API calls do not require a personal GPU.
- Beginners should not buy expensive GPU hardware too early.
- Cloud GPU is useful but can waste money if left running.
- Colab or Kaggle should be tried before paid GPU services.

Needs review:

- CPU and GPU definitions.
- Difference between local GPU and cloud GPU.
- Stop vs terminate behavior on cloud platforms.

Next recommended lesson:

```text
Phase 0 Lesson 4
```
