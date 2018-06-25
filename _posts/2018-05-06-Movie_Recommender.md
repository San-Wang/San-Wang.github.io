---
layout: post
title: Movie Recommender System in Python
excerpt: "Machine Learning - Recommendation System"
modified: 06/05/2018, 1:55
tags: [Python, Flask, NLP, Recommendation System]
comments: true
category: blog
---

## Overview  
A  recommendation system using content-based & collaborative filtering methods.   
Here is a workflow overview about my demo:  
![workflow](/images/Recommender/workflow.png)  

**What it can do:**  
* recommend movies based on movie's **plot** or **cast**(director & main actors and actresses)  
* recommend movies based on **personal taste**  

[Data Source](https://www.kaggle.com/rounakbanik/the-movies-dataset/data)

**methods:**   
* content-based: NLTK, scikit-learn, TFIDF
* collaborative filtering: surprise, pyspark(final demo)

demo: flask(finished), mySQL(finished), Spark(final demo)

Current demo:  
<a href="https://imgflip.com/gif/2cuv3v"><img src="https://i.imgflip.com/2cuv3v.gif" width="500px" height="300px" title="movie recommender demo"/></a>  

Home page:  
![home page](/images/Recommender/HomePage.png)  
About page:  
![about](/images/Recommender/about.png)  
Recommendation example:  
Request Page:  
![Request Page](/images/Recommender/RecommendRequest.png)  
Recommendation Result Page:  
![RecommendResult1](/images/Recommender/RecommendResult1.png)  
![RecommendResult2](/images/Recommender/RecommendResult2.png)  
Best movie genres:  
![ExploreRequest](/images/Recommender/ExploreRequest.png)   
![ExploreResult](/images/Recommender/ExploreResult.png)   




TODO list:   
* [x] Build local host demo website(flask)  
* [x] Connect mySQL with flask
* [ ] Save similarity matrix in mySQL database  
* [ ] Using pyspark library to do collaborative filtering instead of surprise.SVD
