# NLP SENTIMENT ANALYSIS FOR MOVIE REVIEWS

## Table of Content
  * [Demo](#demo)
  * [Overview](#overview)
  * [Data Preprocessing](#data-preprocessing)
  * [Modeling](#modeling)
  * [Technical Aspect](#technical-aspect)
  * [Deployement on Heroku](#deployement-on-heroku)
  * [Directory Tree](#directory-tree)
  * [To Do](#to-do)
  * [Technologies Used](#technologies-used)

## Demo
Link: http://rottenpineapple.herokuapp.com/](http://rottenpineapple.herokuapp.com/)

https://user-images.githubusercontent.com/37875797/116399793-ee0df000-a846-11eb-82ef-8cd667a13968.mp4




## Overview
This is a simple NLP flask model trained on the imdb dataset for movie sentiment analyzing.
When a user submits a review the app should use the sklearn model trained on the IMDB
dataset to classify the review as positive or negative . The results should be returned to the user  and the result should
display the prediction as either positive or negative.All the movie reviews submitted by users should be stored in a SQLite database together with
the prediction (if it was a positive or negative review).

## Data Preprocessing
Text preprocessing is traditionally an important step for natural language processing (NLP) tasks. It transforms text into a more digestible form so that machine learning algorithms can perform better.In this problem we done following types of preprocessing.
 * Removing all urls from data.
 * Removing all tags from data
 * Decontracting the words
 * Removing special character from data
 * Removing stop words
 * Stemming and Lemmatization
 * Tf-idf vectorization
 
##  Modeling
Imdb dataset is trained mainly on 3 machine learning models
* Logistic Regression
* Navie Bayes
* Support Vector Machine

we got maximum accuracy in the support vector machine, almost 89%.

## Technical Aspect
This project is divided into two part:

1) Training imdb dataset using machine learning models
2) Deployement of model

* For training purposes, we use sklrean library.
* For deployment, we use Flask and Heroku.
* We also database for storing the input and prediction value

## Deployement on Heroku
<img target="_blank" src="https://imgur.com/39Y8cOt.jpg" width=900>

For more information read this [Heroku Documentation](https://devcenter.heroku.com/articles/getting-started-with-python) to deploy a web app.

## Directory Tree
```
├── app 
│   ├── __init__.py
│   ├── app.py
│   ├── model
│   ├── static
│   └── templates
|   └── database.db
|   └── database_init.py
| 
├── config
│   ├── __init__.py
├── processing
│   ├── __init__.py
├── Procfile
├── README.md
└── model.pickle
```
## To Do
* Train data using deep learning models.
* Adding movies options in web app

## Technologies Used
![](https://forthebadge.com/images/badges/made-with-python.svg)

<img src="https://img.shields.io/badge/Machine Learning%20by-SKLEARN-blue.svg"/> 
 <img src="https://img.shields.io/badge/flask%20-%23000.svg?&style=for-the-badge&logo=flask&logoColor=white"/> 
 <img src="https://img.shields.io/badge/SQLite-07405E?style=for-the-badge&logo=sqlite&logoColor=white"/> 
  <img src="https://img.shields.io/badge/Heroku-430098?style=for-the-badge&logo=heroku&logoColor=white"/> 
