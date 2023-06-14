# Background
The Happy Valley Bank in Hong Kong is working on a marketing campaign to promote a new saving deposit subscription plan to their own clients. 
The marketing campaign, like some of those done before, are to be based on phone calls as much as possible. 
Experience shows that they probably need more than one contact with the same clients, hence some are contacted more than once.
The bank has collected anonymized data of their clients whom they have previously contacted by the relationship manager, some with previous similar campaigns, or on other banking businesses. 
# Dataset
17 attributes, including 10 object attributes. 
# Goal
To make use of the dataset to predict if the client will subscribe (or not subscribe) to the new term saving deposit plan in order to inform the bank’s management executive.
# Process
## Exploratory Data Analysis
Classify the 17 indicators in the data set into 5 parts: 
1. Client Basic Information, 
2. Client Financial Information, 
3. Client Contact Information, 
4. Campaign Information, 
5. Target Value. 

Three Dimensional Analysis:
univariate analysis of the distribution of a single variable, 
bivariate analysis of the relationship between target values and variables,
multivariate analysis combined with target values and different variables. 
Through the detailed EDA analysis, provide the data insights to the marketing team with relevant suggestions for the next marketing activities.

## Three Machine Models: Random Forest, LightGBM, MLP
### Model Selection-Random Search and Grid Search
Build machine learning models to predict the outcome of this marketing campaign. In this project, three machine learning models were built, including Random Forest, LightGBM, and MLP, to predict the outcome of a marketing campaign. 
Feature selection was conducted using RFE and correlation filtering to improve the accuracy of predicting customer subscription. 

Model selection was performed by tuning hyperparameters using Random Search and Grid Search. 
### Imbalanced Dataset Handling
The highly imbalanced dataset was addressed by focusing on precision, recall, F1 value, and AUC value, and using different methods for each model. After adjusting for the unbalanced data, the recall of the models significantly improved, but the AUC decreased. 
## Result
The ensemble learning voting classifier was used to combine Random Forest and LightGBM models, resulting in the best performance with a Precision value of 0.56, Recall value of 0.73, F1 Score of 0.64, and AUC value of 0.935.
