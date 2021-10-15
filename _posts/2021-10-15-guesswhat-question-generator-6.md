---
layout: post
title: "Question Generator - Human-Like Visual Dialogue Strategy"
date: 2021-10-15
---
Taking the leap forward from the [previous post](https://sodhinchu.github.io/2021/10/12/guesswhat-question-generator-5/), what are the other startegies humans follow? It is found that, we, humans usually follow confirmation-driven strategies when searching for an information (or) learning a new language.  Inspired by this theory, a new approach is proposed to converse and locate object(s) in GuessWhat game. The blog post discusses about the paper [Looking for Confirmations: An Effective and Human-Like Visual Dialogue Strategy](https://arxiv.org/pdf/2109.05312.pdf).

> Authors: Testoni et al <br/>
> Published: at EMNLP 2021 <br/>
> Github Repo: [Looking for Confirmations](https://github.com/albertotestoni/confirm_it) <br/>

- Core Idea: Having an internal oracle as part of question generator, that guides to ask questions that reinforces guesser's beliefs
- Focus is on dialogue strcuture rather on surface level features used by RL approaches
- Task accuracy increased y 4.35% with Confirm-it reranking module
- More natural and effective dialogues than beam search decoding without re-ranking


The proposed architecture and the sample dialogue are given below<br/>

<img src="/images/confirmit_arch.png" alt="questioner_arch" class="inline" width="40%" height="10%"/> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
<img align="centre" src="/images/confirmit_sample.png" alt="results" class="inline" width="40%" height="100%"/>


**Authors observations:**<br/>
- The dialogues created by the baseline beam search containing questions on entities which are not present in images<br/>
- By following up on a single object through the dialogues, the repetitions, hallucinated entities are reduced
- This method can be easily extended to other task-oriented dialogue systems which involve generating questions


**Implementation Details:**
- Image: Encoded with ResNet-152 Network
- Dialogue History: LSTM Network
- Question Generator: Uses Greedy Search to generate questions
- ConfirmIt: Internal Oracle, part of Question Generator module, to confirm the beliefs
  - A beam search, re-ranking algorithm
  - Model generates dialogues of 5 turns
  - Uses beam size of 3
  - Val Accuracy: 51.49


#visual #dialog #confirmit #guesswhat #task-oriented	
