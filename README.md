# Neural_Network_Charity_Analysis

## Overview
This machine learning and neural network analysis is being done to determine a binary classifier that is capable of predicting whether applicants will be successful if funded by a company Alphabet Soup.
From Alphabet Soup’s business team, we received a CSV containing more than 34,000 organizations that have received funding from Alphabet Soup over the years. Within this dataset are a number of columns that capture metadata about each organization.

## Results
### Data Preprocessing
-	We have considered the variable IS_SUCCESSFUL as a target for the model
-	For the feature we have considered the below listed variables
    - APPLICATION_TYPE—Alphabet Soup application type
    - AFFILIATION—Affiliated sector of industry
    - CLASSIFICATION—Government organization classification
    - USE_CASE—Use case for funding
    - ORGANIZATION—Organization type
    - STATUS—Active status
    - INCOME_AMT—Income classification
    - SPECIAL_CONSIDERATIONS—Special consideration for application
    - ASK_AMT—Funding amount requested
-	We have excluded the variables EIN and NAME—Identification columns as they do not contribute to the Model.

### Compiling, Training, and Evaluating the Model
-	We have used the deep learning models as it can identify patterns, determine severity, and adapt to changing input data from a wide variety of data sources. Compared to basic neural network models, which require a large number of neurons to identify nonlinear characteristics, deep learning models only need a few neurons across a few hidden layers to identify the same nonlinear characteristics.
-	Neurons. Used approx. 2 to 3 times of the total variables of features which are 43
    - hidden_nodes_layer1 = 80
    - hidden_nodes_layer2 = 30
-	Layers Used
    - Features - 2 Hidden Layer
    - Target - 1 Layer
-	Activation Functions
    - Features – Relu
    - Target - Sigmoid
-	We got an accuracy of 72% which is above average but no satisfactory.
-	We tried following steps to improve model performance.
    - Changed the neurons to 90 and 40

![](Resources\Optimize_attempt_1_hidden_nodes.png)


    - Changed the epoch from 50 to 100



    - Changed the activation from “relu” to “linear”



## Summary
-	The deep learning model with and without optimization could yield a performance accuracy of 70 to 75%
-	This is an above average performance but not optimal. Anything above 80% can be summarised as a good performance accuracy to predict whether applicants will be successful if funded by Alphabet Soup.
-	My recommendation will be to use SVM or Random forest model to determine the accuracy of performance as these models are faster and can predict the performance faster. They may have a similar output but can be considered as an option by adding more data to improve the prediction.
