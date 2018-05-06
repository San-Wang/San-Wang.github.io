---
layout: post
title: Movie Recommender System in Python
excerpt: "Machine Learning - Image Classification"
modified: 05/06/2018, 1:55
tags: [Python, Flask, NLP]
comments: true
category: blog
---

## Overview  
A  recommendation system using content-based & collaborative filtering methods.  
**What it can do:**  
* recommend movies based on movie's plot & keywords  
* recommend movies based on cast: director & main actors and actresses  

[Data Source](https://www.kaggle.com/rounakbanik/the-movies-dataset/data)

methods: 
* content-based: NLTK, scikit-learn, TFIDF
* collaborative filtering: surprise, pyspark(final demo)

demo: flask(finished), mySQL(final demo), Spark(final demo)

Current demo:  
<a href="https://imgflip.com/gif/29fzmi"><img src="https://i.imgflip.com/29fzmi.gif" width="500px" height="300px" title="movie recommender demo"/></a>  
  
Home page:  
![home page](/images/Recommender/HomePage.png)  
About page:  
![about](/images/Recommender/about.png)  
Recommendation example:  
![example](/images/Recommender/example.png)


TODO list:   
* [x] Build local host demo website(flask)  
* [ ] Add mySQL to store similarity matrix 
* [ ] Use pySpark machine learning library to implement collaborative filtering  
* [ ] Save similarity matrix in mySQL database  
* [ ] Using pyspark library to do collaborative filtering instead of surprise.SVD
