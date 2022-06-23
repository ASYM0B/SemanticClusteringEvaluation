# Evaluation of Semantic-base Clustering using Asym0b
## Introduction
ASYM0B (A framework for SYsteMatically assessment Of chatBots) is a framework to analyse and assess conversational agents or chatbots built in different tools. To support chatbots from different platforms, ASYM0B relies on a neutral chatbot definition called [CONGA](https://saraperezsoler.github.io/CONGA/).
In this [link](https://github.com/ASYM0B/tool) there are ASYM0B environments, which can be used with these chatbots files. 

This repository contains the data of a experiment to evaluate a Semantic-base Clustering of chatbots using Asym0b. To perfome the experiment we use 259 chatbots created
by third parties, from two differents tecnologies (Dialogflow and Rasa) and three sources code repositories like Github, predefined chatbots from the Dialogflow and Rasa platforms, and predefined chatbots from other platforms like [Kommunicate](https://www.kommunicate.io/). The complete dataset of the experiment is available in this [link](https://github.com/ASYM0B/Dataset). 

## Manual Labeling

In a first step, we manually labelled each of the chatbots. At the end of this process we obtained 43 groups, including 6 with only one element (singletons). Each label
represented a semantic field such as “hotels”, “basic conversations” or “food”. A chatbot can be classified using more than one label. For example a chatbot that offers services for searching restaurants is labelled both with “search” and “restaurant”. 
The following table shows the result of the labeling:


