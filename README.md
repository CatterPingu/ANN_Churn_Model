# Churn Prediction using Artificial Neural Networks (ANN)

This project is focused on building an Artificial Neural Network (ANN) model for predicting churn rate of bank customers. The dataset used in this project is "Churn_Modelling.csv".

## Dataset

The dataset has the following columns:

RowNumber
CustomerId
Surname
CreditScore
Geography
Gender
Age
Tenure
Balance
NumOfProducts
HasCrCard
IsActiveMember
EstimatedSalary
Exited


## Data Preprocessing

The following steps were taken for preprocessing the dataset:

Splitting the dataset into independent (X) and dependent (y) variables.
One hot encoding the categorical variables Geography and Gender.
Concatenating the one hot encoded variables to the independent variable X.
Dropping the original categorical variables Geography and Gender.
Splitting the dataset into train and test data.
Feature scaling the independent variables using StandardScaler.

## Model Building

The ANN model was built using Keras library.

The ANN model consists of an input layer with 6 neurons, a hidden layer with 6 neurons and an output layer with 1 neuron.
The activation functions used for the input and hidden layer were ReLU.
The activation function used for the output layer was sigmoid.
The model was compiled using Adamax optimizer and binary_crossentropy loss function.
The model was fit on the train data using batch size of 10 and 100 epochs.
Dropout regularization was not applied to any layer in this project.


## Model Evaluation

The model was evaluated using the following steps:

The accuracy and loss of the model were plotted for both train and test data.
Confusion matrix was calculated to evaluate the performance of the model.
Accuracy score was calculated using the predicted values and test data.

## Results

The accuracy score of the model was found to be 0.86, indicating that the model performed well in predicting the churn rate of bank customers.

## Conclusion

The Artificial Neural Network (ANN) model developed in this project can be used by banks to predict the churn rate of their customers, which can help them to take necessary actions to retain customers.
