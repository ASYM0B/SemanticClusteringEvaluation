# Evaluation of Semantic-based Clustering using Asym0b
## Introduction
ASYM0B (A framework for SYsteMatically assessment Of chatBots) is a framework to analyse and assess conversational agents or chatbots built in different tools. To support chatbots from different platforms, ASYM0B relies on a neutral chatbot definition called [CONGA](https://saraperezsoler.github.io/CONGA/).
In this [link](https://github.com/ASYM0B/tool) there are ASYM0B environments, which can be used with these chatbots files. 

This repository contains the data of an experiment to evaluate a Semantic-based Clustering of chatbots using Asym0b. To perform the experiment we use 259 chatbots created
by third parties, from two different tecnologies (Dialogflow and Rasa) and three source code repositories like Github, predefined chatbots from the Dialogflow and Rasa platforms, and predefined chatbots from other platforms like [Kommunicate](https://www.kommunicate.io/). The complete dataset of the experiment is available in this [link](https://github.com/ASYM0B/Dataset). 

## Manual Labeling

In the first step, we manually labelled each of the chatbots. Each label represented a semantic field such as “hotels”, “basic conversations” or “food”. A chatbot can be classified using more than one label. For example, a chatbot that offers services for searching restaurants is labelled both with “search” and “restaurant”. The following table sumaries the manual clustering. We obtained 43 groups, including 6 with only one element (singletons), the maximun number of labels in one chatbot is 3, and the maximun number of elements with the same label is 32 (label BASIC). 

<table class="tg">
<thead>
  <tr>
    <th class="tg-7zrl"></th>
    <th class="tg-8d8j">Manual<br> Clustering</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td class="tg-7zrl">#Labels / #Clusters</td>
    <td class="tg-8d8j">43</td>
  </tr>
  <tr>
    <td class="tg-7zrl">Max labels per chatbot</td>
    <td class="tg-8d8j">3</td>
  </tr>
  <tr>
    <td class="tg-7zrl">#singleton cluster</td>
    <td class="tg-8d8j">6</td>
  </tr>
  <tr>
    <td class="tg-7zrl">Min elements</td>
    <td class="tg-8d8j">1</td>
  </tr>
  <tr>
    <td class="tg-0lax">Max elements</td>
    <td class="tg-baqh">32</td>
  </tr>
  <tr>
    <td class="tg-0lax">Avg. elements</td>
    <td class="tg-baqh">7.7</td>
  </tr>
  <tr>
    <td class="tg-7zrl">Median elements</td>
    <td class="tg-8d8j">5</td>
  </tr>
</tbody>
</table>

In the folder Manual Labeling, you can find a table, as well as an excel file, with the results of the manual labelling. 
To compare the clusters labelled manually with the ones created by the algorithm. we defined the clustering matrix as follows. Let C = {c1, ..., cn} the set of chatbots,
then MC is the clustering matrix of C if:
* MCij = 1 if ci and cj share a cluster.
* MCij = 0 otherwise.

The complete matrix is available in the Manual Labeling folder. 

## Asymo0b Clustering

In the second phase, we apply hierarchical clustering to the same set of chatbots, switching between six linkage methods between the clusters (average, centroid, complete, single, median and weighted) and the distance threshold value chosen to form the clusters from 0.01 to 0.99 with 0.01 steps. The lower the threshold is, the higher is the amount of clusters. The following table shows a summary of the best clustering found by our method (method weighted with 0.97 of threshold), which yield 29 clusters having between 1 and 43 chatbots. Clusters have an average of 9.2 and a median of 15 elements, and there are 3 singleton clusters.

<table class="tg">
<thead>
  <tr>
    <th class="tg-7zrl"></th>
    <th class="tg-8d8j">Agglomerative<br>Clustering<br></th>
  </tr>
</thead>
<tbody>
  <tr>
    <td class="tg-7zrl">#Labels / #Clusters</td>
    <td class="tg-8d8j">29</td>
  </tr>
  <tr>
    <td class="tg-7zrl">Max labels per chatbot</td>
    <td class="tg-8d8j">1</td>
  </tr>
  <tr>
    <td class="tg-7zrl">#singleton cluster</td>
    <td class="tg-8d8j">3</td>
  </tr>
  <tr>
    <td class="tg-7zrl">Min elements</td>
    <td class="tg-8d8j">1</td>
  </tr>
  <tr>
    <td class="tg-0lax">Max elements</td>
    <td class="tg-baqh">43</td>
  </tr>
  <tr>
    <td class="tg-0lax">Avg. elements</td>
    <td class="tg-baqh">9.2</td>
  </tr>
  <tr>
    <td class="tg-7zrl">Median elements</td>
    <td class="tg-8d8j">15</td>
  </tr>
</tbody>
</table>

Folder Asym0b Clustering contains an excel file for each method, with all the matrix for each value of the threshold. 

