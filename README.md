# Neural_Network_Charity_Analysis

## Overview of the analysis: 

The purpose of this analysis is to create a machine learning model that can accurately predict success for a given charity application.

## Results:

### Data Preprocessing:

#### What variable(s) are considered the target(s) for your model?

 - We are attempting to predict the variable IS_SUCCESSFUL for a given data point.

#### What variable(s) are considered to be the features for your model?

 - APPLICATION_TYPE,	AFFILIATION	CLASSIFICATION,	USE_CASE,	ORGANIZATION,	STATUS,	INCOME_AMT,	SPECIAL_CONSIDERATIONS,	ASK_AMT

#### What variable(s) are neither targets nor features, and should be removed from the input data?

 - EIN and ID

### Compiling, Training, and Evaluating the Model:

#### How many neurons, layers, and activation functions did you select for your neural network model, and why?


The original code had 2 hidden layers with 8 and 5 neurons.  This resulted in a model with appx. 73% accuracy.  A model with 3 hidden layers and 8,6,4 neurons resulted in the same outcome.  Finally, when a fourth hidden layer was added and the neurons were increased to 40,20,10,5, the outcome was only 72%.  Playing with activation functions and changing one to tanh did not affect the outcome.

#### Were you able to achieve the target model performance?

No.

#### What steps did you take to try and increase model performance?
After increasing the hidden layers to 3 and changing the neurons to 8, 6, and 4, as well as changing the activation function of the added hidden layer to tanh, the model was no better at predicting the outcome.  Additionally, when all other non-numeric columns were removed, the accuracy of the model dropped to approximately 63%.  Even when a fourth layer was added with many more neurons, the outcome was no better.

## Summary: 

It appears that more work would need to be done to fit a neural network model to this data.  I did attempt to run an SVM model, but my machine lacks the processing power to complete it.  A random forest model proved slightly less accurate than a neural network at 70% accuracy.  The next step would be to evaluate variable weights with the data to clean it in a more intentional manner, then re-try the neural network.
