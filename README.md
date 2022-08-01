# Neural Network Charity Analysis

## Project Overview

This project uses deep learning neural networks to analyze and classify the success of charitable donations. The TensorFlow Python library is used for this analysis.

## Results

### Data Preprocessing

- The "EIN" and "NAME" columns are for identification and were removed.
- The column "IS_SUCCESSFUL" was used as the target for the model.
- The "APPLICATION_TYPE", "AFFILIATION", "CLASSIFICATION", "USE_CASE", "ORGANIZATION", "STATUS", "INCOME_AMT", and "SPECIAL_CONSIDERATIONS" were used as the model features.
- The features were encoded, split into training and testing sets, and standardized for the model.

### Compiling, Training, and Evaluating the Model

- The initial model uses two hidden layers with 80 and 30 neurons activated using ReLU.
- Sigmoid is used for the output layer since the target is binary.
- The initial model had an accuracy of 73.1%.
- Three methods were used in an attempt to improve model accuracy above 75%. Each attempted method built on the previous attempt.
 - Increasing hidden layer neurons to 100 and 50 with model accuracy of 72.6%.
 - Adding a third hidden layer with 30 neurons with model accuracy of 72.9%.
 - Changing hidden layer activation function to tanh with model accuracy of 73.0%.

## Summary
The deep learning neural network was unable to achive a baseline of 75% accuracy. With this problem being a binary classification a Random Forest Classifier machine learning model can be used and evaluated against the deep learning model used in this project.