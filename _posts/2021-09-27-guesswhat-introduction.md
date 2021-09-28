---
layout: post
title: "GuessWhat?!: An Introduction To The Task-Oriented Visual Dialogue Systems"
date: 2021-09-27
---
### What?
Task-oriented visual dialogue systems aim to identify an object from a given complex visual scene, through a series of yes/no questions. The core idea is to enable machines to have natural conversations with humans.

### Why?
Naurally conversant systems are more transparent, interpretable and is useful in many real-life situations. The biggest challenge of these systems is understanding natural language questions and perceiving them in visual world. <br/>

### How?
Visual dialogue systems work at the intersection of Computer Vision and Natural Language Processing. GuessWhat?! is a two-player game developed with a focus to stimulate this research area. Deeper understanding of the visual scene, strategy to generate questions, achieving the task success are key components of the system. In this game, both the players get to see a visual scene containing multiple objects. One player: The Oracle randomly assigns an object in the scene which is unknown to second player. The second player, Questioner need to identify the object through a series of questions. For all the questions, Oracle answers in yes/no and its Questioner's responsibility to keep track of the answers and generate the next questions accordingly.<br/>

![image info](/images/Example_Image.png)
<br/>
<br/>
The above image is taken from the paper [de Vries et al](https://arxiv.org/pdf/1611.08481.pdf). It shows how Oracle and Questioner converses and arrives at the answer.<br/>

### Dataset
GuessWhat?! dataset consists of 150K human-played games with a total of 800K visual question-answer pairs on 66K images.<br/>

### Research Focus
With the increase in interest towards natural conversations between machine and humans, multimodality started seeing big push from researchers. There are numerous works that are focusing on enhancing the performance of questioner, having a seperate module for guesser, reducing the repetetion of questions, devising a strategy to generate questions and many more.  <br/>
In the coming posts, would like to dwell more on to these sub-tasks and discuss my understandings. <br/>

#visual #dialog #task-oriented #guesswhat
