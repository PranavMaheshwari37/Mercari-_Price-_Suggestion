# Mercari_Price_Suggestion

## Introduction

Mercari is an online selling Application(Japan) . Sellers upload the products that they want to sell. While uploading , the sellers want to see the price of the products they should be selling at.
Given details about a product like product category name, brand name, and item condition, the challenge is to find an algorithm which predicts the price.
It can wipe up the labors used for maintaining the price and also this can increase the efficiency of the Shopping App.
The mission is to predict the price given the features/attributes of a particular product.

## Machine Learning Formulation

Given details about a product like product category name, brand name, and item condition, Can you build an algorithm that automatically suggests the right product prices? Quite challenging, right?
But if solved rightly, it can eliminate human interference in giving price suggestions of a product and speed up efficiency of the shopping app. That’s when Machine Learning comes to play.

## Data set 

I've taken dataset from kaggle (https://www.kaggle.com/c/mercari-price-suggestion-challenge/data).In The data set there are seven features which are described below.

1.) Name: The name of the product that is being listed by the seller.

2.) Item condition id: A number that represents the condition of the product.

3.) Category: The product category which are in a 3 level hierarchy splitted by ‘/’ and i am going to split it as Main _Category/Subcategory1/..

4.) Brand: The brand of the product.

5.) Shipping: This feature contains boolean variables in which 1 represents the price of shipping is paid by the seller and the other represents the shipping price is paid by                 the buyer.

6.) Item Description: This feature contains the detailed description of the product , their working conditions , all the details that a buyer should know. This is a very                               important feature and most of the Machine Learning and Deep Learning algorithms consider text feature as an important one and this feature can let the NLP                       tasks to come and join in our travel.

7.) Price: This is the value to be predicted and this contains values in the range 0 to 2009

## Performance Metric

Root Mean Square Logarithmic Error(RMSLE).

RMSLE is the best metric for a regression task. For a product, it is okay to predict a higher price value and but it is not worthy to predict a lower price value for the same. RMSLE will increase if we under predict and it will decrease if we over predict. Go through the documentation below to get a better understanding.
