# Quora question-pairing

## Description
This project was part of Natural Language Processing (NLP: CS 6120) under Prof. Ahmad Uzair in summer 2022.

### Problem statement
The problem is to find two sentences with similar meaning. There are lots of examples over the internet which require filtering the sentences based on uniqueness in the meaning. For instance, there could be many reviews or emails or text documents which involve restructuring of sentences and yet provide same meaning to it.
For this purpose, we found a dataset on Kaggle which provides information if two questions posted on quora have similar meaning or not. The set of labels that have been supplied by human experts. However, human labeling is a noisy process as people can have conflict on agreement. As a result, the labels on this dataset are taken as is but not 100% accurate.

### Dataset
> https://www.kaggle.com/competitions/quora-question-pairs/data

## Steps
- EDA ( Exploratory Data Analysis )
- Preprocessing
- XGBoost with word level TF-IDF
- XGBoost with n-gram level TF-IDF
- XGBoost with char level TF-IDF
- BERT model
- Performance Measures and Evaluation.

### EDA and Pre-processing
#### Dataset
- Data contains: 404290 rows and 3 columns
- First Column: Question_1 (string)
- Second Column: Question_2 (string)
- Third Column: Label (0 or 1)

<img src="https://github.com/shah-fo/quora-question-pairing/tree/main/img/dataset.png" width="100px">

#### Histogram
- Log histogram depicting count of occurence of each question

<img src="https://github.com/shah-fo/quora-question-pairing/tree/main/img/eda_histogram.png" width="100px">

#### Density Plot
- Density plot of duplicate and non duplicate questions. Plot is between word count ratio and density.

<img src="https://github.com/shah-fo/quora-question-pairing/tree/main/img/eda_density_plot.png" width="100px">

#### Word Cloud
- Word Clouds can be good icebreakers and can provide an entry point for a topic of discussion.

<img src="https://github.com/shah-fo/quora-question-pairing/tree/main/img/eda_word_cloud.png" width="100px">

### BERT Model
- BERT stands for Bidirectional Encoder Representations from Transformers, which is a type of neural network model used in Natural Language Processing (NLP). It is a type of pre-trained language model that uses a large amount of unlabeled text data to learn the context of words in a language. BERT helps to understand the nuances of language and the relationships between different words and phrases.

<img src="https://github.com/shah-fo/quora-question-pairing/tree/main/img/bert_model.png" width="100px">

### Evaluation

<img src="https://github.com/shah-fo/quora-question-pairing/tree/main/img/evaluation.png" width="100px">

### Libraries
- pandas
- pytorch
- scikit-learn
- numpy
- matplotlib
- seaborn

## Other Contributors
- Dhavan Sanghvi (https://github.com/Dhavan05)
- Nidhi Bodar ()