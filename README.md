# NLP SENTIMENT ANALYSIS FOR MOVIE REVIEWS

## Table of Content
  * [Demo](#demo)
  * [Overview](#overview)
  * [Preprocessing](#preprocessing)
  * [Modeling](modeling)
  * [Technical Aspect](#technical-aspect)
  * [Deployement on Heroku](#deployement-on-heroku)
  * [Directory Tree](#directory-tree)
  * [To Do](#to-do)
  * [Technologies Used](#technologies-used)



## Overview
This is a simple NLP flask model trained on the imdb dataset for movie sentiment analyzing.
When a user submits a review the app should use the sklearn model trained on the IMDB
dataset to classify the review as positive or negative . The results should be returned to the user  and the result should
display the prediction as either positive or negative.All the movie reviews submitted by users should be stored in a SQLite database together with
the prediction (if it was a positive or negative review).
