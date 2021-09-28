---
layout: post
title: "GuessWhat?!- Available Datasets (1/2)"
date: 2021-09-28
---
Predominantly for the task-oriented visual dialogue systems, the [GuessWhat dataset](https://github.com/GuessWhatGame/guesswhat#data) has been in use. However, with the rise in popularity, new datasets have been proposed periodically to further up the game. This post(part-1 of 2 posts) discusses the present-day datasets for these systems.<br/>


## GuessWhat:
The dataset was first introduced in the paper: [Guesswhat?! visual object discovery through multi-modal dialogue](https://arxiv.org/pdf/1611.08481.pdf)
<br/>

**Images**: A filtered subset of [MS COCO dataset](https://cocodataset.org/#home) images are used. Images that contain three to twenty objects are only used to ensure the conversation neither trivial nor complex.<br/>
In total, 77,973 images consisting of 609,543 objects are used for dataset curation.<br/>

**Dialogues**: Two seperate tasks are created on AMT for the questioner and oracle roles. After pre-processing, validation, final dataset Consists of 155,280 dialogues containing 821,889 question/answer pairs on 66,537 unique images and 134,073 unique objects. <br/>
All questions have binary answers (yes/no/na) and distributed as 52.2% No, 45.6% Yes, 2.2% NA <br/>

**Answers**: Binary (Yes/No/NA)<br/>

The baseline code is available [here](https://github.com/GuessWhatGame/guesswhat) <br/>

An example from the dataset is shown below<br/>
![image info](images/gw_sample.png)
<br/>
<br/>
<br/>
## VisDial
The dataset was introduced in the paper: [Visual Dialog](https://arxiv.org/pdf/1611.08669.pdf)<br/>

**Images**: Collected from [MS COCO dataset](https://cocodataset.org/#home). The visual complexity of these images allows for engaging and diverse conversations <br/>
<br/>
**Dialogues**: Two persons chat on AMT with real-time conversations about the image with the roles of questioner and answerer. 

**Answers**: Not restricted to short/concise, but as naturally and as conversationally possible. <br/>

Overall, VisDial contains 1 dialog each (with 10 question-answer pairs) on ∼140k images, for a total of ∼1.4M dialog question-answer pairs.<br/>

Dataset can be downloaded from [here](https://visualdialog.org/data) <br/>
The source code for the [dataset curation](https://github.com/batra-mlp-lab/visdial-amt-chat) and paper are available [here](https://github.com/satwikkottur/visdial-1)<br/>

An example from the dataset is shown below<br/>
![image info](images/vid_sample.png)
<br/>
<br/>
<br/>
## AVSD (Audio Visual Scene Aware Dialog)
The dataset was introduced in the paper: [Audio Visual Scene-Aware Dialog](https://arxiv.org/pdf/1901.09107.pdf)<br/>

**Videos**: Collected from [Charades human-activity dataset](https://prior.allenai.org/projects/charades). The visual complexity of these images allows for engaging and diverse conversations <br/>
<br/>
**Dialogues**: Two persons chat on AMT with real-time conversations about the events in the video with the roles of questioner and answerer. 

**Answers**: Provides as detailed answers as possible. <br/>

Overall, ACSD dataset contains  11816 conversations (7985 training, 1863 validation, and 1968 testing), each including a video summary. There are a total of 118,160 question/answer (QA) pairs<br/>

Dataset can be downloaded from [here](https://video-dialog.com/) <br/>
The baseline code is available [here](https://github.com/hudaAlamri/DSTC7-Audio-Visual-Scene-Aware-Dialog-AVSD-Challenge)<br/>

An example from the dataset is shown below<br/>
![image info](images/avsd_sample.png)
<br/>
<br/>
<br/>
#datasets #visual #dialog #task-oriented
