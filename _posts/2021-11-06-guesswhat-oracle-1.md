---
layout: post
title: "Oracle - Region under Discussion for Visual Dialog"
date: 2021-11-06
---
Majority of the previous works in task-oriented systems, question generator used dialogue history to generate the next question in the conversation. So far, the understanding was dialogue history, along with answers aided in anticipating the best probable future question. There is also a [paper](https://arxiv.org/pdf/2010.00361.pdf) on answer-driven visual estimation to improve the task success rate. However there is not much analysis on how the dialogue history is impacting the oracle's responses. How oracle can use dialog history? This is the theme for today's blog post. The blog post discusses about the paper, [Region under Discussion for visual dialog](https://aclanthology.org/2021.emnlp-main.390.pdf)
<br/>

> Authors: Mazuecos et al <br/>
> Published: at EMNLP-2021 <br/>
> Github Repo: [Region under Discussion for visual dialog](https://github.com/mmazuecos/Region-under-discussion-for-visual-dialog)
<br/>

- Core Idea: Analysis of dialogue history and its impact on Oracle modelling
- Proposes a novel interpretable representation that visually grounds dialog history
- Two Oracle models are extended (i) Question+Category+Spatial (QCS) baseline  (ii) LXMERT-based cross-modal Oracle (CMO)
- QCS+RuD and CMO+RuD show an increment of 41% and 46% respectively
- Released a manually annotated subset of history dependent questions


The proposed architecture and the sample dialogue are given below<br/>

<img src="/images/region_under_discussion_architecture.png" alt="region_under_discussion_architecture" class="inline" width="50%" height="20%"/> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
<img align="centre" src="/images/region_under_discussion_results.png" alt="region_under_discussion_results" class="inline" width="40%" height="100%"/>


**Authors observations:**<br/>
- Spatial, color and size questions are relative and can have their meaning changed due to the RuD (Region Under Discussion) <br/>
- Visual questions dependent on dialog history do not contain more pronouns and ellipses than history independent visual questions
- RuD is capturing the region of the image on which the history dependent question is being interpreted
- Many of these history dependent questions come from an object question that has already identified the category of the target object and now are looking for another salient object to univocally identifying it.
- Only a low percentage of questions (12%) are indeed history dependent in the Guess what?! dataset

#visual #dialouge #hallucinations #guesswhat #task-oriented	
