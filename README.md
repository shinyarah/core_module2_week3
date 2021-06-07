# core_module2_week3
week 3 IP
DEFINING THE QUESTION
a) Specifying the question
As a data analyst for Nairobi Hospital

build models to determine whether or not the symptoms presented by patients indicate hypothyroid

b) Defining the metric for success
This will be achieved when we get the best performing kernel between linear, polynomial and rbf

c) Understanding the context
Using either random forests, ada boosted trees or gradient boosted trees, document the setting up of parameteres to identify which two models that determine the features that are most impactful in influencing the prediction
Apply Polynomial, linear and rbf kernel function to build your SVM model and then evaluate their performance and pick the kernel that performs the best. Remember to tune your parameters to improve the performance of your model. To make your life easier, make sure to visualize the models you've created. Use any two features to build the models for this step.
d) Experimental design
Data cleaning
Perform EDA
Build the random forest classifier
Build the gradient booster classifier
Build the linear function
Build the polynomial function
Build the rbf model
[1]
#importing libraries
import pandas as pd
import numpy as np

#loading dataset
forth=pd.read_csv('/content/hypothyroid (1).csv')
forth.head()

[2]
forth.tail()

[3]
forth.shape
(3163, 26)
[4]
forth.dtypes
status                       object
age                          object
sex                          object
on_thyroxine                 object
query_on_thyroxine           object
on_antithyroid_medication    object
thyroid_surgery              object
query_hypothyroid            object
query_hyperthyroid           object
pregnant                     object
sick                         object
tumor                        object
lithium                      object
goitre                       object
TSH_measured                 object
TSH                          object
T3_measured                  object
T3                           object
TT4_measured                 object
TT4                          object
T4U_measured                 object
T4U                          object
FTI_measured                 object
FTI                          object
TBG_measured                 object
TBG                          object
dtype: object
