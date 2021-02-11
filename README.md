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
  - Were you able to achieve the target model performance?
  - What steps did you take to try and increase model performance?

## Summary
Summerarize the overall results of the deep learning model. Include a recommendation for how a differenct model could solve this classification problem, and explain your recommendation.
