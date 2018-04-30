---
layout: post
title: Bais Variance Tradeoff
published: true
---
Machine Learning is all about creating the models ,But when we try create models we encounter many errors and one of the most important error in machine learning which is called **Bais Variance Tradeoff**

Bais Variance Tradeoff can be broke down into three part :
- Bais
- variance
- irreducible error

These are the three errors often happend when we try to create a model
Let's understand what these  errors are and how we can control it

## What Is Bais error ?
![baiserror.png]({{site.baseurl}}/images/baiserror.png)

Bais error occur when we make simplifying assumption.
In this picture above the points are scattered in the 2D plane between size and price in the first image, We have created a simple plane to seprate the points but this plane is unable to seprate these point ,Here we are making the simplefiying assumpting that causing High Bais which ultimately leads to **Underfitting**

Let's Take Another Example of K nearest neighbour to understand bais error more clearly

![baiserror.png]({{site.baseurl}}/images/20nearestneigh.png)

Image shown above shows the decision boundary between positive and negative point since the value of k = 20 
the descision boundary is more smoother , but we can see that as we increase the value of k the decision boundary is become more smoother and will utimately increase the Bias error that result in **underfitting**

## What is Variance error ?
![baiserror.png]({{site.baseurl}}/images/baiserror.png)

When ever we work on any data set we used to seprate the training data , cross validation data and the test data .We use training data to train the model for future unseen data but if any small change in the training data completely changes the model than it means we have **high variance error** which result in overfitting

In the above image  the data point scatter in the 2D plane. In third image we can see that plane is overfitting the points that result in **High Variance error** which lead to overfitting problem 

## Relationship between Variance and Bias error?

![baiserror.png]({{site.baseurl}}/images/baisvariance.png)

Above Image show the 2D graph between Error and Model Complexity and  by looking at this we can clearly Understand the relationship between variance and bias 

When the Model complexity is minimum that means less than the **optimal model complexity line** the variance is small and the bias is very high ,Where as when the Model complexity is maximum that means higher than the **optimal model complexity line** result in high variance and small bias.

From the above graph we can see that as the model complexity increases or we can say that in knn when k decreses from higher value than bais decreses sharply as we can see in the graph and variance increases slowly  but after the optimal k value when k decreases furthermore the variance increases sharply and bias decreases slowely .











