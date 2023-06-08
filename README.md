# Insurance
Project using an example Insurance dataset taken from the book 'Machine Learning with R'
(https://github.com/stedy/Machine-Learning-with-R-datasets/blob/master/insurance.csv).
A regression analysis is performed on the dataset using a simple Neural NEtwork build in TensorFlow 2.X.

# This project uses:
* TensorFlow 2.X to create, train and evaluate the performance of a regression dataset
* Sequential API to build a simple neural network composed of 4 fully-connected Dense layers
* Normalisation and one-hot encoding of data

The dataset contains information regarding a person's health insurance in America, with values based on metrics such as a person's age, sex, BMI, whether they smoke or not, the number fo chilren they have and the region of the country they are from. The model created aims to predict that given a person's details, how much the person's insurance would cost.

The dataset is split into an 80:20 split of trainign data to test data. The model validated using the test data during the training of the model.

The numerical data is normalised to be between 0 and 1 using `MinMaxScalar()` and the non-numerical data is one-hot encoded.

# Evaluation
* On the training data, the model achieves a MAE of 3476.62
* On the test data, the model achieves a MAE of 3168.44
