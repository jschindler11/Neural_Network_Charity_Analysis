# Neural_Network_Charity_Analysis

## Overview of the analysis

We created two binary classifiers that are capable of predicting whether charitable organization applicants will be successful if funded the foundation 'Alphabet Soup.'

## Results

### Data Preprocessing
* Every variable apart from "IS_SUCCESSFUL" are the targets for our model (Note: for our AlphabetSoupCharity notebook, we dropped the non-beneficial ID columns ("EIN" and "NAME." For our AlphabetSoupCharity_Optimization notebook, we dropped the "EIN" column but not the "NAME" column, and instead decided to bin organization names with less than five appearances in the dataset in an attempt to optimize our model and increase our accuracy score).
* The variable "IS_SUCCESSFUL" is considered the feature for our model

### Compiling, Training, and Evaluating the Model
* In both models, we used two hidden layers and an output layer
* In both models, hidden layer one had 80 neurons and hidden layer two had 20 neurons
* In both models, we used the 'relu' activation function for hidden layers one and two, and the 'sigmoid' activation function for our output layer

We aimed to achieve at least a 0.75 accuracy score for our model

The accuracy score of our first model (in the AlphabetSoupCharity notebook) was 0.7259474992752075

<img width="609" alt="Screen Shot 2023-01-28 at 7 24 50 PM" src="https://user-images.githubusercontent.com/111151454/215303070-def17f3b-b647-4169-aa2a-efba31036b7c.png">

The accuracy score of our second model (in the AlphabetSoupCharity_Optimization notebook) was 0.7885714173316956

<img width="609" alt="Screen Shot 2023-01-28 at 7 25 01 PM" src="https://user-images.githubusercontent.com/111151454/215303106-f0f557e0-ee8b-40eb-8cf3-47b77a31dfce.png">

* As mentioned above, by binning organziation names with less than five appearances in the dataset, we were able to increase the model performance, resulting in an accuracy score increase of 0.06262391805


## Summary

Binning organization names with less than five appearances in the dataset resulted in a more optimized model. We created a model that successfully achieved our accuracy score of at least 0.75. I reccomend creating a Random Forest machine learning model for this dataset, as this type of model is generally less influenced by outliers.

