# Capstone Project: Create a Customer Segmentation Report for Arvato Financial Services

### Overview
In this project, I analyze demographics data for customers of a mail-order sales company in Germany and I compare it against the demographics of the broader Germany population to identify people that are most likely to become customers. This is done in a few different stages:
- Data Exploration/Preparation: The first third of the workbook is geared around data exploration and preparation for machine learning algorithms. Here we develop an understanding for the data we will be working with, drop columns that have too many missing records, drop rows without enough metadata, re-encode columns not in the right format and eliminate highly correlated variables. We finish by imputing missing data points and scaling the features so we can use an unsupervised learning algorithm for further analysis.
- Unsupervised Learning Algorithm - Once the data is prepared, we can apply Principal Component Analysis to reduce dimensionality, identify the optimal number of kmeans clusters and determine how the customer population differs from the general population from a cluster perspective.
- Supervised Learning Algorithm - Lastly we can implement a supervised learning model to a training set. After we go through the same process of data preparation, we can then test different models to see how well they are able to predict the likelihood of someone becoming a customer. Once the top model is identified, we can train it further to optimize its predictions and ultimately use the model on test data to identify who the best targets are for marketing campaigns and overall customer acquisition.

## Table of Contents
1. Setup/Requirements and Instructions for Running 
2. Files in Repositroy
3. Report and Blog Post
4. Acknowledgements


## Setup/Requirements and Instructions for Running 
requirements.txt has all libraries needed for this workbook
If you just want to run the prebuilt model, import a test set and you can run it through the best_clf.predict_proba function after running through the steps needed to clean the data.


## Files in Repository
There are a number of .csv files for checkpoints where work was saved. These can pretty much be ignored unless you want to load them in at a specific stage to see how the code is functioning at various points.
'Arvato Project Workbook.ipynb' has all of the code in a live jupyter notebook
'Arvato Project Workbook.html' contains the html extract of the notebook
'DIAS Attributes - Values 2017.xlsx' and 'DIAS Information Levels - Attributes 2017.xlsx' have data related to the features used in building the model
'requirements.txt' has all of the requirements for running the notebook
'results.csv' has the results of the model on a test set
'visuals.py' was created by udacity and has visualization functions for supervised learning algorithm outputs

## Blog Post
Report:
- Check out this in depth explanation of all the work that went into this analysis at a techncial level and understand the different approaches that were taken for different modeling efforts: https://github.com/bchase17/DS_Capstone/blob/main/Report.pdf
Blog:
- Check out this high level explanation of what went into this analysis explained in a more simplisitc and easy to digest way: https://github.com/bchase17/DS_Capstone/blob/main/Capstone%20Blog%20Post.pdf

## Acknowledgements

- Through my prior experience with Udacity's Machine Learning nano-degree, I was able to leverage previous project work from my github to build out my supervised and unsupervised algorithms: https://github.com/bchase17/machine_learning/tree/main
