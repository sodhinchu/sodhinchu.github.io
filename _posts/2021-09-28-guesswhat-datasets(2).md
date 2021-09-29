---
layout: post
title: "GuessWhat?!- Available Datasets (2/2)"
date: 2021-09-29
---

In continuation with the previous post, here are some more datasets that are useful to work with Visual Dialogue Systems.<br/>
<br/>
## VFD:
The dataset was first introduced in the paper: [A Visually-grounded First-person Dialogue Dataset with Verbal and Non-verbal Responses](https://aclanthology.org/2020.emnlp-main.267.pdf)
<br/>

**Images**: Used the 34,775 first-person images with eye-gaze annotations in the [GazeFollow dataset](http://gazefollow.csail.mit.edu/download.html).<br/>

**Dialogues**: Yahoo! Crowd Sourcing is used to collect the verbal and non-verbal responses for a given image. A total of 308,793 verbal and 81,867 non-verbal responses are collected after removing noisy/trivial responses. <br/>

The dataset can be downloaded from [here](https://github.com/yahoojapan/VFD-Dataset) <br/>

An example from the dataset is shown below<br/>
![Sample Data](/images/vfd_sample.png)
<br/>U, V, N denote an utterance, a verbal response, and a non-verbal response respectively
<br/>
<br/>
<br/>
## PhotoBook:
The dataset was first introduced in the paper: [The PhotoBook Dataset: Building Common Ground through Visually-Grounded Dialogue](https://arxiv.org/pdf/1906.01530.pdf)
<br/>

**Images**: [MS COCO dataset](https://cocodataset.org/#home) images are used.<br/>

**Dialogues**: Unlike other visual dialogue datasets where a player acts as questioner and other as answerer/guesser, in Photobook Dataset, there are no such roles. Both players converse freely and naturally leading to normal conversation. AMT is used to curate the dialogues. <br/>

The dataset consists of 164,615 utterances, 130,322 actions and spans a vocabulary of 11,805 unique tokens<br/>

The dataset can be downloaded from the [github page](https://dmg-photobook.github.io/datasets.html) and the source code from [here](https://dmg-photobook.github.io/code_models.html).<br/>

An example from the dataset is shown below<br/>
![Sample Data](/images/photobook_sample.png)
<br/>
<br/>
<br/>
## IGC: Event-Centric Conversations on Images
The dataset was first introduced in the paper: [Image-Grounded Conversations: Multimodal Context for Natural Question and Response Generation](https://arxiv.org/pdf/1701.08251.pdf)
<br/>

**Images**: A sample of eventful images from [VQG Dataset](https://www.microsoft.com/en-us/download/details.aspx?id=53670).<br/>

The dataset can be downloaded [here](https://www.microsoft.com/en-us/download/details.aspx?id=55324) and the baseline code from [here](https://github.com/chingyaoc/VQG-tensorflow) <br/>

An example from the dataset is shown below<br/>
![Sample Data](/images/igc_sample.png)
<br/>
<br/>
<br/>
## Image-Chat:
The dataset was first introduced in the paper: [Image-Chat: Engaging Grounded Conversations](https://arxiv.org/pdf/1811.00945.pdf)
<br/>

**Images**: Images are randomly selected from [YFCC100M Dataset](http://projects.dfki.uni-kl.de/yfcc100m/).<br/>

The dataset can be downloaded from [here](parl.ai/projects/image_chat) and the baseline code is available [here](https://github.com/facebookresearch/ParlAI) <br/>

An example from the dataset is shown below<br/>
![Sample Data](/images/imagechat_sample.png)
<br/>
<br/>
<br/>
#datasets #visual #dialog #task-oriented
