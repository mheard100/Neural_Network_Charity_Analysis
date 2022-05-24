# Neural_Network_Charity_Analysis


## Overview of the Analysis 
Beks has come a long way since her first day at that boot camp five years ago—and since earlier this week, when she started learning about neural networks! Now, she is finally ready to put her skills to work to help the foundation predict where to make investments.

With your knowledge of machine learning and neural networks, you’ll use the features in the provided dataset to help Beks create a binary classifier that is capable of predicting whether applicants will be successful if funded by Alphabet Soup.

From Alphabet Soup’s business team, Beks received a CSV containing more than 34,000 organizations that have received funding from Alphabet Soup over the years. Within this dataset are a number of columns that capture metadata about each organization, such as the following:

EIN and NAME—Identification columns
APPLICATION_TYPE—Alphabet Soup application type
AFFILIATION—Affiliated sector of industry
CLASSIFICATION—Government organization classification
USE_CASE—Use case for funding
ORGANIZATION—Organization type
STATUS—Active status
INCOME_AMT—Income classification
SPECIAL_CONSIDERATIONS—Special consideration for application
ASK_AMT—Funding amount requested
IS_SUCCESSFUL—Was the money used effectively


## Results 

### Data Preprocessing 
- Target variable for the model: IS_SUCCESSFUL Column
- Variables that were considered features for my model: Every Column except for IS_SUCCESSFUL which is our target and the ones we will drop (EIN, Name). The dropped features have no impact on the outcome of being successful. 

### Compiling, Training and Evaluating the Model

The target accuracy score for our model was 75%. The model created in the first two deliverables had an accurage of 57%

- Attempt 1: The first change from the model created in the first two deliverables was to add a neuron layer going from 2 to 3. The accurage percentage did not change with the additional layer

- Attempt 2: Adding Additional neurons to the original 2 layers.Layer one had 500 and layer two had 100 neurons when originally we had 80 and 30 respectively. This decreased the accuracy of getting our untrained data correct in the model only 48% of the time.



- Attempt 3: I ran a logistic regression model. This model was chosen because we are trying to solve for a categorical result - is the donation successful or not. The accuracy score increased to 73%. 


## Summary 
The logistic regression model almost hit the 75% accuracy perameter set fourth. The initial neural network had a accuracy score of 57% and did not change or got worse adding neuron layers and neurons. This loss in accuracy can be explained from the fact that the model overfitted. We could further also optimize our neural network by removing more features or simply adding more data to the dataset to increase accuracy. Furthermore, trying new models would be beneficial. Random Forest ensemble is a good model for classification and works well with outliers and nonlinear data. It uses weaker algothorithms to make decision trees and ties them together to make a prediction. This could model could have helped with overfitting and increased efficiency in the algorithms. 
