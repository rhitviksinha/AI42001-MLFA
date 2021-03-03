# LAB 2

## Wednesday, 16<sup>th</sup> September, 2 - 5 PM

# Assignment 2

Lab Assignment 2 *(incomplete submission)*: [Python Notebook](./LAB_ASSIGNMENT_2.ipynb)

The second assignment is **NumPy implementation of Linear Regularization** and **Lasso and Ridge Regressions**.

### Provided Dataset:

Consider the attached dataset ([Advertising Dataset.csv](./Advertising%20Dataset.csv)) about advertising and sales. The attributes denote the investments on advertising in TV, radio etc and the target variable is the total sales. The aim is to predict the sales from the investments on advertising.

200 training examples. 3 features for each example provided.

### Description:

1. Randomly divide the dataset into training (75%) and testing (25%) subsets **[1 mark]**

2. Using Linear Regression, fit a model to predict the sales from investments using your own formula. Compare the coefficients as found by the python library function **[3 marks]**

3. Compute the mean squared error on the testing set **[1 marks]**

4. Using ridge regression with different values of lambda (0.5, 1, 5, 10, 50, 100) plot the coefficients against each other, and also compare the test set mean squared errors. **[3 marks]**

5. Use the library function of "LASSO regression" to find out which of the 3 features is most important, i.e. whose coefficient is furthest from 0. **[2 marks]**
