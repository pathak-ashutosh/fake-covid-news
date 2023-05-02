# FakeCovid Fact Checked News
## Introduction
This project is a requirement of the course CS 584 Data Mining and Applications at GMU, although the idea is novel and the dataset is taken from Kaggle. *[Source](https://zenodo.org/record/3965871#.Y9ZAJdJBwUE)*

## Team Members
- [Ashutosh Pathak]()
- [Chaithra Bekal]()

## Background and Motivation
- The COVID-19 pandemic has been a global crisis that has affected the lives of billions of people worldwide. 
- Misinformation and fake news about COVID-19 have also been a growing concern, leading to public panic and confusion. 
- Our project aims to explore and analyze fake news related to COVID-19 and identify the patterns and characteristics that make it more likely to be shared or believed.

## Project Objectives
- To analyze the characteristics of fake news related to COVID-19 and identify the patterns that make it more likely to be shared or believed.

## Data
- The dataset is taken from [Kaggle](https://www.kaggle.com/datasets/thedevastator/fakecovid-fact-checked-news-dataset).
- The FakeCovid dataset is a compilation of 7623 fact-checked news articles related to COVID-19.
- Obtained from 92 fact-checking websites located in 105 countries, this comprehensive collection covers a wide range of sources and languages, including locations across Africa, Europe, Asia, The Americas and Oceania.

## Questions
- What are the most common topics of fake news related to COVID-19?
- Which countries were most susceptible to fake news, and what were the reasons behind it?
- Which websites were the least accurate sources of news?
- What kind of fake news spreads in a particular country?

## Data Preprocessing
- The dataset was cleaned and preprocessed using Python.
- Extract classes and filter out null values.
- The existing classes were a lot and included ambiguous classes like ‘partially true’, ‘misleading’, ‘half true’ etc.
- We chose 3 broad classes ‘True’, ‘False’ and ‘Uncertain’.
- Countries of origin in a lot of articles are grouped together, so we are splitting and aggregating them to get a better view.
- ‘content’ feature is multilinguistic, using ‘title’ feature instead which is translated to English.

## Models
- We used the following models to classify the news articles:
  - Logistic Regression
  - Random Forest
  - Decision Tree
  - Support Vector Machine
  - K-Nearest Neighbors

## Results
We're using Accuracy Score as the metric to evaluate our models. (this might change in the future)
Before categorizing classes into 3 broad groups we were getting ~0.79.
Accuracy Score:
- Decision Tree = 0.940249
- Random Forests = 0.942219
- Logistic Regression = 0.942875
