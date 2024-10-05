# Report on Neural Network Model 

## Overview of the analysis: 

- In this challenge, I used a CSV file containing 34k+ organizations that have received funding from Alphabet Soup (a charity organization). The goal was to predict if future organizations would be successful. I used machine learning and neural networks with a target accuracy of above 75%, so I will try a few models with different layers and activations to see which seems to work the best. 

## Results: 

### Data Preprocessing

- Imported necessary dependencies 
- Dropped "EIN" and "NAME" columns, because neither of those were targets/features
- Determined the number of unique values in each column
- Identified value counts for replacing
- Used get dummies to convert data to numeric
- Created target variable --> 'IS_SUCCESSFUL' column
- Separated the feature variables --> other columns, once the target column is dropped
- Used StandardScaler to scale the training and testing sets 


### Compiling, Training, and Evaluating the Model


How many neurons, layers, and activation functions did you select for your neural network model, and why?

First Model: 

- 2 hidden layers with 100 neurons each. I chose the activation ReLU for the first two hidden layers because it is simple, efficient, and my data is non-linear. 
- A third output layer with the sigmoid activation.
    - This model got an accuracy of 72.5% and a loss percentage of 57.5%. 

Second Model:
- One hidden layers with 80 neurons. I chose tanh activation for this layers. 
- A second output layer using sigmoid activation. 
    - This model got an accuracy of 73% and a loss percentage of 56%.
- As I tried to add more hidden layers to this one, the accuracy went down so I tried to keep it simple. 

Were you able to achieve the target model performance?

- I was not able to reach target performance of 75%. 

What steps did you take in your attempts to increase model performance?

- In order to increase model performance, I decreased number of neurons per layer, I tried adding layers, removing them, using different activations.. but I still was not able to reach the goal. 

## Summary: 

- In my first model, I may have used too many neurons per layer. To avoid this problem I lowered the number of neurons per layer and used less hidden layers. 
