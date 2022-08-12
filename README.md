# Neural_Network_Charity_Analysis

## Overview of the analysis

With our knowledge of machine learning and neural networks, we used the features in the provided dataset to help create a binary classifier that is capable of predicting whether applicants will be successful if funded by Alphabet Soup. 

From Alphabet Soup’s business team, we received a [CSV]( https://github.com/JaimeStarling/Neural_Network_Charity_Analysis/blob/main/charity_data.csv) containing more than 34,000 organizations that have received funding from Alphabet Soup over the years. Within this dataset are a number of columns that capture metadata about each organization, such as the following:

- EIN and NAME—Identification columns
- APPLICATION_TYPE—Alphabet Soup application type
- AFFILIATION—Affiliated sector of industry
- CLASSIFICATION—Government organization classification
- USE_CASE—Use case for funding
- ORGANIZATION—Organization type
- STATUS—Active status
- INCOME_AMT—Income classification
- SPECIAL_CONSIDERATIONS—Special consideration for application
- ASK_AMT—Funding amount requested
- IS_SUCCESSFUL—Was the money used effectively

## Results

### Data Preprocessing
- The **IS_SUCCESSFUL** column is considered the target as it is very clear, binary, and easy to understand.
- We removed the **EIN** and **NAME** columns as they were unnecessary for the analysis being neither targets nor features.
- The remaining columns are considered to be the features for our model.

![This is an image](https://github.com/JaimeStarling/Neural_Network_Charity_Analysis/blob/main/Images/Application%20DF.png)

### Compiling, Training, and Evaluating the Model

How many neurons, layers, and activation functions did you select for your neural network model, and why?
There were three attempts to achieve a target predictive accuracy higher than 75 percent. One model used hidden layers of 80 neurons and 30 neurons, and the other two models used hidden layers of 100 neurons, 50 neurons, and 20 neurons. Activation functions include *relu*, *sigmoid*, and *tahn*. The idea was to try different training to improve the accuracy of each model. Unfortunately, no model reached the desired 75 percent accuracy.

## Summary

The models, using a machine learning neural network, failed to reach the desired accuracy at three attempts, and would either require far more attempts to get closer to 75 percent or lower the desired accuracy, which is not recommended. There are different models to use with this same data, especially given the **IS_Successful** column, with a *Linear Regression Model* or a *Random Forest Classifier* that are simpler to run and may achieve the accuracy we need.
