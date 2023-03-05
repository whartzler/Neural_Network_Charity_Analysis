# Neural_Network_Charity_Analysis

## Overview
Working with Alphabet Soup a non profit organization to determine which organizations are worth donating to and which are to high risk.  We will be Tensorflow to creating a deep network neural network model to determine which organizations are best to receive donations. 

## Results
### Data Preprocessing
The Target Variable: IS_SUCCESSFUL.  This metric clearly shows weither or not the application is successful. 
The Feature Variables: APPLICATION_TYPE, AFFILIATION CLASSIFICATION, USE_CASE, ORGANIZATION STATUS, INCOME_AMT, SPECIAL_CONSIDERATIONS, ASK_AMT
The removed variables are name and EIN.  These variables do not contribute to the end results if a applicant is successful or not as they are descriptions.

### Compiling, Training, and Evaluating the Model
#### Initial Model
- Layer 1:  80 units as this is close to double our input features of 41
- Layer 2: 40 Units as half of layer 1.  this is a good rule to not overcrowd your model.
Hidden Layers used relu as all our features are from 1 - infinity
Output Layer is sigmoid as we are looking for an output of 1 or 0 identifying yes or no the application will be successful.


#### Optimized Model


## Summary

### Resources

### Application
