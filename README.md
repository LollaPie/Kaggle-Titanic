
# Titanic Kaggle Competition

## Table of Content

1. [Installation](#installation)
2. [Motivation](#motivation)
3. [File Description](#description)
4. [Results](#results)
5. [Acknowledgements & Licensing](#acknowledgements--licensing)

## Installation <a name="installation"/>

Python versions 3.0 or higher is needed. Used Packages in this Juypter Notebook:

- Numpy
- Pandas
- Re
- Matplotlib
- Seaborn
- Sklearn

## Motivation <a name="motivation"/>

This is my solution for the free kaggle Titanic competition. The dataset includes passenger information
like age, name, family member on board, ticket number, etc. and whether they survived or not.
The task is to predict the survival of passengers. For evaluation the accuracy metric is used. Every
competitor has a free choice of how they wrangle the data and which model they use.

## File Description <a name="description"/>

This repository contains only one jupyter notebook. The dataset can be downloaded from [Kaggle](https://www.kaggle.com/competitions/titanic/data) by accepting the competition rules.

## Results <a name="results"/>

I find that the feature engineering is the most important task for this challenge. One can use the surnames and
ticket numbers to find families which are in the train data as well as in the test data. Family member help each
other therefore if one family member survived the chances are high that other members survived as well. Thus you
get more information especially from the test data.

I tried different models on the train data (Logistic Regression, Random Forest, Gradient Boost, SVC, ANN, etc.).
The Gradient Boosting Classifier showed the best results. I used GridSearchCV from sklearn to tune the model.
The accuracy scores are:

- test data: 82,5 %
- train data: 84,7 %
- competition data: 78,47%

This score got my under the top 15% which is a decent result.

## Acknowledgements & Licensing <a name="acknowledgements--licensing"/>

I would like to thank Kaggle for providing this competition. Kaggle is a really great platform to train your skills on machine learning. I am looking forward to future competitions.

Feel free to use the code in this repository for your projects.
