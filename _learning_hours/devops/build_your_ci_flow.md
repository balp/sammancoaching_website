---
theme: devops
title: Build Your CI Flow
difficulty: 1
author: balp
affiliation: HiQ
---

# Build your CI flow

The goal of this lesson is to get discussions on
what to add first in a CI/CD pipeline. What steps are needed 
and what might be more hindrance.

## Requirements

* A collection of cards for different integration, verification and delivery steps.
  For example using the [pipeline game](https://www.eficode.com/pipeline-game).
ª
## Session Outline

* 5 min: Connect: Three facts and a question about CI/CD
* 7 min: Concept: What are the main principles we have when building a CI pipeline
* 20 min: Concrete: Do the pipeline game, make a minimal chain
* 20 min: Concrete: Do the pipeline game, extend the chain for fusa
* 5 min: Conclusions: Is there anything about you CI/CD flow you like to change now

### Connect: Three facts and a question about CI/CD

As a pair, come up with three facts and a question and one
question about CI/CD. Collect the facts into one list, then go
through the questions from each pair. Note these as well and
the goal is that they should be able to answer the questions
after the session.

### Concept: What are the main principles we have when building a CI pipeline

#### Basics of CI/CD

Explain what CI/CD C* is about,
* Continuous Integration -> Get the code to a main, master, branch.
* Continuous Deployment -> Get the code to a production (like) environment.
* Continuous Delivery -> Get the code to a user.

Why? do we do CI/CD.
* Quicker development
* Better results
* Happier developers

Data on devops, in short it's good for business.
Explain some of the conclusions form (The State of Devops)[https://dora.dev]


#### Setting up a CI/CD pipeline

* Make an as small as possible flow from developer to customer.
  In our experience a small flow that starts at the developer and
  ends with the customer, this might be an upstream department, an
  other stakeholder of an external user. Gives us the most value.
* Grow the pipeline.
  After we have established the minimal flow to reach the customer we
  start adding more functionality to increase the confidence in our
  product.
* Thinning the CI/CD flow.
  We need to continuously revisit the flow to reduce or remove steps
  to ensure the feedback is quick enough for the developers.
* Lengthening the CI/CD flow.
  Over time we can change the start or end of our pipeline to include
  other parts of our organization.
* Avoid slow and manual steps?

### Concrete: Design a minimal CI/CD pipeline

Using a deck of cards, either from [the pipeline game](https://www.eficode.com/pipeline-game),
or create your own similar cards adapted to match the customers problems. There might
be some things you feel is need for an embedded or functional safety environment.

As them to create a minimal pipeline that goes from the developer to the customer.
Ask them to keep developer feedback times in mind.

After about 10 minutes ask them to motivate why they choose the start, end points.
If there are any manual or slow steps. Ask them to motivate. They goal is to get
a healthy discussion on what is really needed in the pipeline.  

Example of questions:
* Why is your manual review after the Unit-test? Can you do it earlier at the desktop before committing?
* Do you need a traceable version number for the release? Can it be the commit hash?


### Concrete: Expand the pipeline with FUSA requirements

After about 20 minites into building the pipeline, they usually starts to
feel like they have the minimal flow. Time to spice up the game.

Lets add more requirements:

* The cybersec team are concerned about security issues in the product.
* The FuSa (Functional Safety) team are worried we don't know what we deliver. 

Let them add as little little or much as they like, but be ready to defend there
choices to business (e.g. the coach).

Have them prepared to to answer the following questions: 
* Which one did you add? 
* In what order? 
* What made you choose those? 


### Conclusions: Is there anything about you CI/CD flow you like to change now

Have them sit down in a pair and discuss if there is anything in there
current CI/CD flow they now feel is good to change. 
