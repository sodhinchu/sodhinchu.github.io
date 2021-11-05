---
layout: post
title: "Question Generator - Hallucinating Entities in GuessWhat?!"
date: 2021-11-05
---
True to its title, the paper, [Hallucinating Entities in GuessWhat?!](https://aclanthology.org/2021.acl-srw.11.pdf) brings out how existing question generators hallucinating entities while conversing with the oracle. Hallucination referes to generating words that are not matching with source data. And these hallucinations creating a domino effect in the generated dialogues and degrading the overall quality of the system. Such systems are harmful to deploy in real-world as it persons with viewing disabilities value correctness over the fine-grained descriptions.

The below image showcases the queries for entities that are not existing in the visual scene. <br/><br/><br/>
<img src="/images/hallucinating_examples.png" alt="hallucinating_examples" class="inline" width="40%" height="10%"/> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;


> Authors: Testoni et al <br/>
> Published: at ACL IJCNLP-2021 <br/>

- Core Idea: Stresses the issue of hallucination in visual dialogue (most of these agents have fixed number of questions to ask and with hallucinating questions, the game may end up as failure which impacts the overall accuracy of the system)
- Studies the impact of fine grained visual representations on reducing the hallucinations
- Proposes two Questioner models (i) LXMERT-GDSE (ii) VLP
- Proposes to use CHAIR metric (similar to image captioning) for dialogues


The proposed architecture and the sample dialogue are given below<br/>

<img src="/images/hallucinating_architecture.png" alt="hallucinating_architecture" class="inline" width="40%" height="10%"/> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
<img align="centre" src="/images/hallucinating_percents.png" alt="hallucinating_percents" class="inline" width="40%" height="100%"/>


**Authors observations:**<br/>
- Hallucinations cause a cascade effect <br/>
- Rate of object hallucination increases across the dialogue turns
- Hallucinations are more likely to occur after negative answers
- These models struggle to profit from negatively answered questions, even when they are crucial to succeed in the game
- Proposed model (using VLP) generating hallucinations like humans (generated conversations are similar to human conversations in the dataset)


**Food for thought:**<br/>
- What other strategies can be employed to handle the difficulties faced by multimodal encoders in grounding negation?
- Deeper understanding of the role of negation in visual dialogues (Apart from hallucination, what else they effect?)
- Is there any correlation between hallucinations and repetitions?
- The paper discussed about entity hallucinations only, what other types of (attributues/spatial/..) hallucinations can occur and methods to tackle them

#visual #dialouge #hallucinations #guesswhat #task-oriented	
