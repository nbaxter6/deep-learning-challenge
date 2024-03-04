# deep-learning-challenge

## Report: Neural Network Model
### Overview
The purpose of this analysis is to build a predictive model for the nonprofit foundation Alphabet Soup, that can predict whether an applicant will be successful if they are granted funding. Alphabet Soup’s business team provided a csv containing 34,000 organizations, several features about those organizations, and whether they were successful to build the predictive model on. Using the knowledge I have gained about machine learning from this class, I will attempt to build a neural network model that can meet the needs of Alphabet Soup to select applicants with confidence in their success. 
### Method/Results
First the data was preprocessed by removing irrelevant data and separating the raining data into target and features. 
#### Data that was removed:
•	EIN

•	NAME
#### Features (X):
•	APPLICATION_TYPE

•	AFFILIATION

•	CLASSIFICATION

•	USE_CASE

•	ORGANIZATION

•	STATUS

•	INCOME_AMT

•	SPECIAL_CONSIDERATIONS

•	ASK_AMT

#### Target (y):
•	IS_SUCCESSFUL

After the data was separated into features and target, it was split into the training and testing groups, and then scaled using Standard Scaler. Then the neural network model was compiled and trained. The model consists of two hidden layers with 80 and 20 neurons respectively, and one output layer. The hidden layers used “relu” activation and the output layer used “sigmoid” activation. The model was compiled using “binary_crossentropy” for loss and “adam” optimizer. 
To improve the performance of the model keras_tuner was installed and imported. Then tuner was used to find the best parameters of the model. 
### Summary
The original model had a loss of 56% and an accuracy score of 72.9%. The karas tuner model had a loss of 56% and an accuracy score of 73.2%. I would not recommend using this model as the loss is too high and the accuracy could be further improved. 
