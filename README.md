# Neural_Network_Charity_Analysis

## Overview
In this project, we create a binary classifier with neural networking models to help Alphabet Soup's business team predict which applicants will be worth investing in.  We use a CSV of over 34,000 organizations that have received funding from Alphabet Soup over the years to train and test our model.

## Results
### Data Preprocessing
Before we begin to compile and train our model, we must answer several important questions first:

- Our target variable is "IS_SUCCESSFUL"
- Our features include APPLICATION_TYPE, AFFILIATION, CLASSIFICATION, USE_CASE, ORGANIZATION, STATUS, INCOME_AMT, SPECIAL_CONSIDERATIONS, ASK_AMT
- The variables removed from the data set are name, and identification number: "EIN","NAME"
### Model
Now we must define and adjust our model to optimize performance:
- Our model began with 2 hidden layers- 20 neurons in the first and 10 in the second.  Out activation functions were ReLU by default and sigmoid to end. 
- We did not quite reach 0.75 accuracy in performance
- We added a hidden layer, added neurons throughout, changed the activation functions to tanh, and decreased the number of epochs to 70.


## Summary

We missed our desired accuracy, 75%, by a couple of points.  This means our model accurately predicted successful investments 73% of the time amongst our testing data.  This is an improvement over our original 72%.

I would recommend going back and re-processing the data.  Perhaps more or less features would help train the model.

I would also recommend trying a Random Forest Classifier model.  It is comparable to a neural network model, but may outperform with speed and code efficiency.
