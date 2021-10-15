---
layout: post
title: "Question Generator - Category based question generation strategy"
date: 2021-10-15
---
As can be guessed from the title: [Category-Based Strategy-Driven Question Generator for Visual Dialogue](https://aclanthology.org/2021.ccl-1.89/), this paper uses category based strategy for the question generation

> Authors: Shi et al <br/>
> Published: at CCL 2021 <br/>

- Core Idea: A category based strategy-driven question generator (CSQG)
- A prior probability strategy is introduced based on dialogue history
- Guesser achieved state of the art success rates (51.71%)

The proposed architecture and the results are given below<br/>

<img src="/images/category_arch.png" alt="questioner_arch" class="inline" width="457" height="278"/> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
<img align="centre" src="/images/category_results.png" alt="results" class="inline" width="40%" height="5%"/>

**Authors observations:**<br/>
- The category is changed if the last question receives a positive answer
- 

**Implementation Details:**
- Encode image and dialogue history (using faster-RCNN, multi-layer GRU) to decide the category of the next question to be generated <br/>
- Question is generated based on CSQG strategy
- GRU [Hidden Size: 2400], with only forward direction and 300 embedding dimension
- After concatenation, a feed forward network [two linear layer with ReLU activation]
- 15 epochs, batch size of 128, test set is accuracy is about: 78.5%


#visual #dialog #csqg #guesswhat #task-oriented	
