# Neural_Network_Charity_Analysis

## Overview
Working with Alphabet Soup a non profit organization to determine which organizations are worth donating to and which are to high risk.  We will be Tensorflow to creating a deep network neural network model to determine which organizations are best to receive donations. 

## Results
### Data Preprocessing
The Target Variable: IS_SUCCESSFUL.  This metric clearly shows weither or not the application is successful. 
The Feature Variables: APPLICATION_TYPE, AFFILIATION CLASSIFICATION, USE_CASE, ORGANIZATION STATUS, INCOME_AMT, SPECIAL_CONSIDERATIONS, ASK_AMT

Removed variables are name and EIN.  These variables do not contribute to the end results if a applicant is successful or not as they are descriptions.

### Compiling, Training, and Evaluating the Model
#### Initial Model
- Layer 1:  80 units as this is close to double our input features of 41
- Layer 2: 40 Units as half of layer 1.  this is a good rule to not overcrowd your model.
Hidden Layers used relu as all our features are from 1 - infinity
Output Layer is sigmoid as we are looking for an output of 1 or 0 identifying yes or no the application will be successful.


#### Optimized Model
- Inlcuded the Name column and grouped all names as other with less than 50 counts
- Layer 1 increased units to 100 
- Layer 2 decreassed the units to 30
- Added an additional Layer with 10 units to see if we can increase the Accuracy
Tested different activation layers but with layer 1 relu, layer 2, 3 & Output were all sigmoid.  
Increased Epochs to 100 

Overall the target model performance was achieved through different tests and analysis.  The primary update to the model to increase optimization was including the Name column rather than removing it,  and not having to few of grouped names.  This allowed a lot more data within our model and allowed us to acheive a 76% accuracy rate. 
Minimal gains were seen with adding additional units to each layer and activation functions.

## Summary
Overall with the data provided we will have an accuracy of 76% to predict if an applicant will succeed or not.  For this case 76% is still low and this model will not do a good job at making sure Alphabet Soup will be contributing its money to the correct applicants.    

Another model that could solve this classification problem would be Random Forest.  This model similar to the Neural Network Model can easily digest large datasets and can handle outliers and nonlinear data.  For this test we did not see if there were any outliers thats where the Random Forest calculator could improve this model. 

### Resources
- AlphabetSoupCharity_Optimizations - Optimized NN Model
- AlphabetSoupCharity - Initial NN Model

### Applications
- Tensorflow for NN Modeling
- Pandas for data upload and processing
