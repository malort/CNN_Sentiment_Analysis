# CNN_Sentiment_Analysis
Sentiment analysis (also known as opinion mining or emotion AI) is the use of natural language processing (NLP), text analysis, computational linguistics and biometrics to systematically identify, extract, quantify, and study affective states and subjective information. 

## Data:

The dataset is a collection of thousands of tweets and their correspondent sentiment label. It is provided by CrowdFlower.

## Requirements:

```pandas:``` Data analysis and manipulation tool.

```spacy:``` is an open-source software library for advanced natural language processing.

```string:``` Common string operations module.

```re:``` This module provides regular expression matching operations

```nltk:``` The Natural Language Toolkit is a suite of libraries and programs for symbolic an statistical natural language processing (NLP).

```keras:``` Open-source software library that provides a Python interface for artificial neural networks. Keras acts as an interface for the TensorFlow library

```scikit-learn:``` Machine Learning library.


## Description: 

### First part: Preprocess and cleaning data. 

Common data cleaning steps as tokenization or lemmatization are performed to prepare the data.


### Second part: Deep Learning solution. 




![imagen](https://user-images.githubusercontent.com/20369543/153262928-6777a2ce-25b5-4012-815d-4d6a36ecd1a2.png)

The architecture used is an n-gram CNN model. The model uses three parallel convolutional neural networks that read the data using different kernel sizes. 
Each channel is composed of the following elements: 
- Input layer that defines input sequences length. 
- Embedding layer set to the vocabulary size. 
- Conv1D layer with 32 filters and a kernel size set to the number of words to read at once. 
- Dropout1D layer as regularization measure. 
- MaxPooling1D layer to consolidate the output from the convolutional layer. 

The outputs from the three channels are concatenated into a single vector and processed by a Dense layer and an output layer.

The following plot depicts the model created.



![imagen](https://user-images.githubusercontent.com/20369543/153263396-abac8a85-bc88-439a-ac57-7e7013934b4a.png)
