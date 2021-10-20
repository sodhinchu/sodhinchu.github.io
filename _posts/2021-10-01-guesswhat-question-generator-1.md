---
layout: post
title: "GuessWhat?!- Question Generator"
date: 2021-10-10
categories: "visual dialogue"
---

While there are numerous research directions in task-oriented systems, I am picking the **question generator** for my reading task, as it is the crucial component in continuing the dialogue. Please check these posts ([introductory paper](https://sodhinchu.github.io/2021/10/01/guesswhat-baselines/), [available datasets](https://sodhinchu.github.io/2021/09/29/guesswhat-datasets(2)/)) for a overview of task-oriented systems.

## Question Generator:
It's role is to continue the conversation by generating questions until the *guesser* module is confident of making a guess to locate the object. Since the total number of questions has an impact on the task success rate, the module should also be mindful on the total number and type of generated questions.<br/>
```bash
Input: Previous dialogs (question history) + Visual Scene
Output: A Question
```
The [base model](https://sodhinchu.github.io/2021/10/01/guesswhat-baselines/) uses HRED(Hierarchical recurrent encoder decoder) by conditioning with VGG features of image<br/>
 ![Question Generator Model](/images/base_model_qgen.png)
 
 

The common problems observed in question generation are:<br/>
- Repeated questions
- Non-coherent questions
- Dialogues are not natural like humans
- Only generating categorical and spatial question
- Models do not learn linguistic skills<br/><br/>



> Here are some of the research papers I found interesting and will be discussing in the coming blog posts.<br/>
>
> 1. [Category-Based Strategy-Driven Question Generator for Visual Dialogue](https://aclanthology.org/2021.ccl-1.89.pdf)
> 2. [Looking for Confirmations: An Effective and Human-Like Visual Dialogue Strategy](https://arxiv.org/abs/2109.05312)
> 3. [Enhancing Visual Dialog Questioner with Entity-based Strategy Learning and Augmented Guesser](https://arxiv.org/pdf/2109.02297.pdf)
> 4. [Unified Questioner Transformer for Descriptive Question Generation in Goal-Oriented Visual Dialogue](https://arxiv.org/pdf/2106.15550.pdf)
> 5. [Visual Dialogue State Tracking for Question Generation](https://arxiv.org/pdf/1911.07928.pdf)
> 6. [Beyond task success: A closer look at jointly learning to see, ask, and guesswhat](https://arxiv.org/pdf/1809.03408.pdf)


<br/>

For following latest research on task-oriented systems,[tune into this an awesome repo](https://github.com/jokieleung/awesome-visual-question-answering) that is curating the papers on visual question answering and visual dialogue

#question #generator #visual #dialog #task-oriented
