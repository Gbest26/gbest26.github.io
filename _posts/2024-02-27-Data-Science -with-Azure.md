---
layout: post
title: Data Science on Azure
subtitle: Learning data science on azure machine learning workspace.
categories: Python
tags: [azure, data science, certificate]
---

## The Azure Machine Learning WorkSpace
1. Create an Azure Machine Learning workspace:
   Before creating a machine learning resource, you need to have a subscription either student, free or paid subscription, after get the subscription next is to create a resource group than automatically comes with a blob storage resource and within the resource group you can create the azure machine learning resource
2. Identify Azure Machine Learning resources:
   Inside the ML workspace you will find other resources like:
   i. the workspace
   ii. the compute resource
   iii. datastore
3. Identify Azure Machine Learning assets:
   ML assets are what data scientist will need while in azure ML workspace and assets are:
   i. Model
   ii. Environment
   iii. Data
   iv. Components

## Automate ML Model Selection
1. Introduction-
   Going through trial and error to find the best performing model can be time-consuming. Instead of manually having to test and evaluate various configurations to train a machine learning model, you can automate it with automated machine learning or AutoML.
   
2. Preprocess data and configure featurization:
  Before running an auto ML you need to configure it first like-
  i. Configure optional featurization
  ii. Understand scaling and normalization
3. Run an Automated Machine Learning experiment:
   there are different model you can run on auto ML like:
   i. Linear regression
   ii. Logistic Regression
   iii. Random forest
   iv. Decision tree, etc.

## Deploy and Consume Models with AML
1. Introduction:
   Imagine you trained a model to recommend restaurants. The model has been trained and tracked in Azure Machine Learning. You want to use the model in your application where consumers can browse restaurants in their area. Each time a consumer selects a restaurant in the application, you want the model to recommend other restaurants that might also be of interest to the consumer to improve the user experience.
2. Explore managed online endpoints:
   To make a machine learning model available for other applications, you can deploy the model to a managed online endpoint.
   i. Real-time predictions
   To get real-time predictions, you can deploy a model to an endpoint. An endpoint is an HTTPS endpoint to which you can send data, and which will return a response (almost) immediately.
   ii. Deploy your model

   Model assets like the model pickle file, or a registered model in the Azure Machine Learning workspace.

   Scoring script that loads the model.

   Environment which lists all necessary packages that need to be installed on the compute of the endpoint.

   Compute configuration including the needed compute size and scale settings to ensure you can handle the amount of requests the endpoint will receive.
## Deploy your MLflow model to a managed online endpoint
1. Deploy an MLflow model to an endpoint
   When you deploy an MLflow model to a managed online endpoint, you don´t need to have the scoring script and environment.
## Deploy a model to a managed online endpoint
1. Deploy a model to an endpoint
   To deploy a model, you must have:
   Model files stored on local path or registered model.
   A scoring script.
   An execution environment.
## Test managed online endpoints
1. Use the Azure Machine Learning studio
   You can list all endpoints in the Azure Machine Learning studio, by navigating to the Endpoints page. In the Real-time endpoints tab, all endpoints are shown.
