---
layout: post
title: Avito Product Demand Prediction  
excerpt: "Machine Learning - Image Classification"
modified: 08/03/2018, 11:20
tags: [Machine Learning, NLP, Computer Vision]
comments: true
category: blog
---  



# Avito Product Demand Project  

[Data Source](https://www.kaggle.com/c/avito-demand-prediction/data)  

## 1. dataset structure  
    * item_id - Ad id.
    * user_id - User id.
    * region - Ad region.
    * city - Ad city.
    * parent_category_name - Top level ad category as classified by Avito's ad model.
    * category_name - Fine grain ad category as classified by Avito's ad model.
    * param_1 - Optional parameter from Avito's ad model.
    * param_2 - Optional parameter from Avito's ad model.
    * param_3 - Optional parameter from Avito's ad model.
    * title - Ad title.
    * description - Ad description.
    * price - Ad price.
    * item_seq_number - Ad sequential number for user.
    * activation_date- Date ad was placed.
    * user_type - User type.
    * image - Id code of image. Ties to a jpg file in train_jpg. Not every ad has an image.
    * image_top_1 - Avito's classification code for the image.
    * deal_probability - The target variable.


## 2. methods to preprocessing each type  
    2.1. text  
    2.2. images  
    2.3. time series    
    

#### 2.1 text data

* stemming
* tf  
* tf-idf  
* text statistics (#words, #char, caps, alphanum)  

#### 2.2 image data 

[reference](https://www.kaggle.com/c/avito-demand-prediction/discussion/59880#349563)  
* image features
    * top predict categories(percentage encoding)
    * [key point detection](https://www.kaggle.com/c/avito-demand-prediction/discussion/59414)(similar idea as ROI)  
    
* [image quality](https://www.kaggle.com/shivamb/ideas-for-image-features-and-image-quality)
    * dullness
    * whiteness  
    percentage of dark(<dark_threshold)/bright(>light_threshold) pixel  
    * uniformity(edge present percentage)
    * dominant color/average color  
    pixel frequency  
    * size
    * blurrness(Variation Laplacian)  
    * [classification confidence](https://www.kaggle.com/wesamelshamy/high-correlation-feature-image-classification-conf)  
    [pipeline](https://www.kaggle.com/peterhurford/image-feature-engineering)  

#### 2.3 Time Series   

* day
* period

Note:  
A interesting way to encode numeric variables using percentage, like price, item_seq_number:  
log1p(price) and log1p(item_seq_number)


## 3. challenges
    * Random Forest takes forever to tune parameters 
        Solution: change to [lightGBM](https://www.microsoft.com/en-us/research/wp-content/uploads/2017/11/lightgbm.pdf)
    * Images size exceeded memory  














