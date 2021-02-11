# Neural_Network_Charity_Analysis

## Overview of Analysis
Using knowledge of machine learning and neural networks create a binary classifier that is capable of predicting whether applicants will be successful if funded by Alphabet Soup. There are four deliverables on this project:
  - Preprocessing Data for a Neural Network Model
  - Compile, Train, and Evaluate the Model.
  - Optimize the Model
  - Written Report on the Neural Network Model

### Resources
- Data Source: [Charity_data.csv](https://github.com/stephenanayashilliard/Neural_Network_Charity_Analysis/blob/main/Resources/charity_data.csv)
- Tools:
 - Python 3.6.1
 - Pandas
 - Neural Network
 - sklearn
  - model_selection
    - train_test_split
  - preprocessing 
    - StandardScaler
    - OneHotEncoder
  - os
  - tensorflow

## Results of Analysis
- ### Data Processing
  - What variables are considered the targets for the model?
    - The target variable for the model is under the column "IS_SUCCESSFUL".  This column determines if a charity used their grants successfully. 
  - What variables are considered to be features for model?
    - The variables that are considered to be features of the model are:
      - Application Type
      - Affiliation
      - Classification
      - Use_Case
      - Organization
      - Status
      - Income Amt
      - Special Considerations
      - Ask Amount
  - What variables are neither targets nor features, and should be removed from the input data?
    - The following variables were not considered as either targets or features and were removed from the data:
      - EIN
      - Name
      
- ### Compiling, Training, and Evaluating the Model
  - How many neurons, layers, and activation functions did you select for your neural network model, and why?
    - Intitial Model:
    The final number of features for the model was around 42.  For the intial evaluation I chose two hidden layers, the first hidden layer contained 40 neurons, the second hidden layer contained 5 neurons. "relu" was the activation used on this first model. 
      - Accuracy
        ![Initital Model](https://github.com/stephenanayashilliard/Neural_Network_Charity_Analysis/blob/main/Resources/Intitial_Model.png)
    - First Attempt:
    For this attempt, I kept the same number of hidden layers and neurons but changed the activation on the hidden layers to "tanh". 
      - Accuracy
        ![1st attempt](https://github.com/stephenanayashilliard/Neural_Network_Charity_Analysis/blob/main/Resources/1st_Attempt.png)
    - Second Attempt:
    For this attempt I increased the number of hidden layers and divided the original 45 neurons between the 3 hidden layers. Returned Activation to "relu" for the three hidden layers.
      - Accuracy
        ![2nd Attempt](https://github.com/stephenanayashilliard/Neural_Network_Charity_Analysis/blob/main/Resources/2nd_Attempt.png)
    - Third Attempt:
    For the third attempt I used the same three hidden layers and number of neurons I used in the second attempt.  I changed the activation for the three hidden features to "sigmoid" and increased the Epoch to 100.
      - Accuracy
        ![3rd_Attempt](https://github.com/stephenanayashilliard/Neural_Network_Charity_Analysis/blob/main/Resources/3rd_Attempt.png)
    
  After three attempts the accuracy did improve but only in extremely small increments.

## Summary
Overall the results of my three attempts were not impressive. I believe that there maybe messy data however, because of many of the columns are coded, I am not aware of what the codes stand for and cannot be sure if they are lessoning the accuracy of the models.
