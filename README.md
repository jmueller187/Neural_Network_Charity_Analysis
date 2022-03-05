# Neural_Network_Charity_Analysis
Explore and implement neural networks using the TensorFlow platform in Python

## Overview of the analysis:
For this project we were tasked with using the Tensorflow platform to build neural networks and deep learning networks in order to analyze a nonprofit foundation dataset. We were able to use the features in the provided dataset to design binary classifiers, which were then used to predict whether applicants will be successful if funded by the foundation.

## Results:
The dataset included a number of columns captured metadata about each organization as shown below:
![Dataset Columns](https://github.com/jmueller187/Neural_Network_Charity_Analysis/blob/main/Resources/DatesetColumns.png)

We used this data to address the following questions:

### Data Preprocessing<br>
#### 1.What variable(s) are considered the target(s) for your model?
- We chose the IS_SUCCESSFUL column of the dataset at the model target, as this column listed whether or not the money received by an organization was used effectively.

#### 2. What variable(s) are considered to be the features for your model?
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

#### 3. What variable(s) are neither targets nor features, and should be removed from the input data?
- We chose to remove the EIN and NAME columns from the input data as they were identification columns and did not contain data that would contribute to our overall analysis

### Compiling, Training, and Evaluating the Model<br>
#### 4. How many neurons, layers, and activation functions did you select for your neural network model, and why?

#### 5. Were you able to achieve the target model performance?

#### 6. What steps did you take to try and increase model performance?

## Summary: Summarize the overall results of the deep learning model. Include a recommendation for how a different model could solve this classification problem, and explain your recommendation.
