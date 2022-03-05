# Neural_Network_Charity_Analysis
Explore and implement neural networks using the TensorFlow platform in Python

## Overview of the analysis:
For this project we were tasked with using the Tensorflow platform to build neural networks and deep learning networks in order to analyze a nonprofit foundation dataset. We were able to use the features in the provided dataset to design binary classifiers, which were then used to predict whether applicants will be successful if funded by the foundation.

## Results:
The dataset included the following columns of captured metadata about each organization:

![Dataset Columns](https://github.com/jmueller187/Neural_Network_Charity_Analysis/blob/main/Resources/DatesetColumns.png)

We used this data to address the following questions:

### Data Preprocessing -<br>
#### 1. What variable is considered the target for your model?
- We chose the IS_SUCCESSFUL column of the dataset at the model target, as this column listed whether or not the money received by an organization was used effectively.

#### 2. What variables are considered to be the features for your model?
- The features of our model included these columns:
    - APPLICATION_TYPE
    - AFFILIATION
    - CLASSIFICATION
    - USE_CASE
    - ORGANIZATION
    - STATUS
    - INCOME_AMT
    - SPECIAL_CONSIDERATIONS
    - ASK_AMT

#### 3. What variables are neither targets nor features, and should be removed from the input data?
- We chose to remove the EIN and NAME columns from the input data as they were identification columns and did not contain data that would contribute to our overall analysis

### Compiling, Training, and Evaluating the Model -<br>
#### 4. How many neurons, layers, and activation functions did you select for your neural network model, and why?
- For our initial neural network model, we chose to use 80 neurons in the first hidden layer and 30 neurons in the second hidden layer. These quantities were used to supply neurons at approximately 2 times and 0.75 times the number of input features in layer 1 and layer 2 respectively.

#### 5. Were you able to achieve the target model performance?
- The target predictive accuracy for model performance was 75%. In our initial evaluation, we were unable to meet the target model performance, as our model accuracy ended up being 72.6%.<br>
![Initial Evaluation Results](https://github.com/jmueller187/Neural_Network_Charity_Analysis/blob/main/Resources/InitialEvaluationResults.png)

#### 6. What steps did you take to try and increase model performance?
- We made four attemps to increase model performance:
        - Attempt 1: Increased neurons in each hidden layer - Layer 1 = 100 neurons, Layer 2 = 50 neurons<br>
        - Result: Model accuracy = 72.7%<br>
        ![Optimization Attempt 1](https://github.com/jmueller187/Neural_Network_Charity_Analysis/blob/main/Resources/OptimizationAttempt1.png)

        - Attempt 2: Added third hidden layer to create deep learning model-
            - Layer 1 = 3 X's number of input features<br>
            - Layer 2 = 1 X's number of input features<br>
            - Layer 3 = 0.5 X's number of input features<br>
        - Result: Model accuracy = 72.5%<br>
        ![Optimization Attempt 2](https://github.com/jmueller187/Neural_Network_Charity_Analysis/blob/main/Resources/OptimizationAttempt2.png)

        - Attempt 3: Changed the model activation function - Ran the deep learning model using the Tanh activation function<br>
        - Result: Model accuracy = 72.5%<br>
        ![Optimization Attempt 3](https://github.com/jmueller187/Neural_Network_Charity_Analysis/blob/main/Resources/OptimizationAttempt3.png)

        - Attempt 4: Increased the deep learning model Epochs to 200<br>
        - Result: Model accuracy = 72.5%<br>
        ![Optimization Attempt 3](https://github.com/jmueller187/Neural_Network_Charity_Analysis/blob/main/Resources/OptimizationAttempt4.png)

## Summary: 
After making four attempts at optimizing our model, we were unable to increase our model performance above the 75% target accuracy, as each of our optimization attempts ended up with an accuracy just under 73%. We would recommend either performing additional preprocessing on the input in case other variables or outliers are causing model confustion or attempt using a non neural network model such as a Support Vector Machine or Random Forest to evaluate the data. The data we evaluated might be of a size and structure that is better suited for the supervised machine learning models and result in improving our target model performance.
