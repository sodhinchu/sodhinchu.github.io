---
layout: post
title: "Natural Language Processing Toolkits For Indian Languages"
date: 2021-06-14
---

Indian Diaspora is rich in languages. According to a 2018 survey, 9 out of 10 new internet users will be Indian language users. Moreover, close to 70% of people consume content in local languages. With the rise in demand, enthusiasts, freelancers and organisations started focusing on developing NLP tools for the Indian languages.
<br/><br/>
This post aims in sharing the existing set of NLP tools and their usage
<br/>

(i) <b> [iNLTK](https://inltk.readthedocs.io/en/latest/) </b> <br/>
NLTK is a pretty popular package available for ENG language analysis. iNLTK is its Indian cousin for analysing regional languages.

<b> Installation </b>
```bash
pip install torch==1.3.1+cpu -f https://download.pytorch.org/whl/torch_stable.html
pip install inltk
```
<b> Setup </b>
```bash
from inltk.inltk import setup
setup('<code-of-language>') // for telugu -> setup('te')
```
The setup is for the first time to use the language that downloads the necessary models for analysis <br/>

<b> Supported Languages </b>
Hindi, Punjabi, Gujarati, Kannada, Malayalam, Oriya, Marathi, Bengali, Tamil, Urdu, Nepali, Sanskrit, English, and Telugu <br/>
It also supports few code-mixed varieties viz., Hinglish (Hindi + Eng), Tanglish (Tamil + Eng), and Manglish (Malayalam + Eng) <br/>

<b> Supported Features </b>
```bash
Tokenize
Get embedding vectors
Predict next 'n' words
Identify language
Remove foreign languages
Get Sentence Encoding
Get Sentence Similarity
Get Similar sentences
```
For more documentation, please visit [here](https://inltk.readthedocs.io/en/latest/)

(i) <b> [IndicNLP](https://indicnlp.ai4bharat.org/home/) </b> <br/>
IndicNLP stemmed from the efforts of the open source community: AI4Bharat. Check out this [page] (https://ai4bharat.org/) for knowing more about the initiative and the projects they are working on <br/>

<b> Installation </b>
```bash
pip install indic-nlp-library

# download the repo
git clone https://github.com/anoopkunchukuttan/indic_nlp_library.git

#download the resources
git clone https://github.com/anoopkunchukuttan/indic_nlp_resources.git
```
<b> Setup </b>
```bash
import sys
from indicnlp import common 
# The path to the local git repo for Indic NLP library
INDIC_NLP_LIB_HOME=r"indic_nlp_library"	 
# The path to the local git repo for Indic NLP Resources	 
INDIC_NLP_RESOURCES=r"indic_nlp_resources"	 
# Add library to Python path	 
sys.path.append(r'{}\src'.format(INDIC_NLP_LIB_HOME))	 
# Set environment variable for resources folder	   
common.set_resources_path(INDIC_NLP_RESOURCES)
#Loads the library
indicnlp.loader.load()
```
The setup is for the first time that sets the necessary resources for analysis <br/>

<b> Supported Languages </b>
Assamese, Bengali, English, Gujarati, Hindi, Kannada, Malayalam, Oriya, Punjabi, Tamil and Telugu <br/>
It also supports few code-mixed varieties viz., Hinglish (Hindi + Eng), Tanglish (Tamil + Eng), and Manglish (Malayalam + Eng) <br/>

<b> Supported Features </b>
```bash
Text Normalisation
Script Information
Word Tokenization and Detokenization
Sentence Splitting
Word Segmentation
Script Conversion
Transliteration
Translation
Syllabification
Indicization
```
For more documentation, please visit [here](https://indic-nlp-library.readthedocs.io/en/latest/index.html) <br/>

(iii) <b> [StanfordNLP](https://stanfordnlp.github.io/stanza/index.html) </b> <br/>

<b> Installation </b>
```bash
pip install stanfordnlp
```
<b> Setup </b>
```bash
import stanfordnlp
stanfordnlp.download('te') #Downloading Telugu lang model
```
<b> Supported Languages </b>
Hindi, Tamil, Telugu and Urdu are supported <br/>

For more documentation, please visit [here](https://stanfordnlp.github.io/stanza/usage.html) <br/>
