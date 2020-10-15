# LAB 5

## Wednesday, 14<sup>th</sup> October, 2 - 5 PM

# Assignment 5

The third assignment is **Handwritten Digit Classification** with **Ensemble Methods**.

### Dataset

**[MNIST handwritten digits dataset](http://yann.lecun.com/exdb/mnist/)** : The MNIST database of handwritten digits, available from this page, has a training set of 60,000 examples, and a test set of 10,000 examples. It is a subset of a larger set available from NIST. The digits have been size-normalized and centered in a fixed-size image.

It is a good database for people who want to try learning techniques and pattern recognition methods on real-world data while spending minimal efforts on preprocessing and formatting.

![MNIST Image](https://upload.wikimedia.org/wikipedia/commons/2/27/MnistExamples.png)

### Description:

1. Download the MNIST handwritten digit dataset. It contains `28×28` images. Flatten them into 784-dimensional binary vectors. Keep aside 20% data for testing and another 20% for validation. **[1 mark]**

2. Now, draw a random subset of 10 dimensions (out of 784). Based on these 10 dimensions only, build a decision tree (using library function). Maximum depth allowed: 5. Calculate accuracy of the tree on validation set. **[2 mark]**

3. Repeat this process for 50 random subsets like this, each of dimension 10.For each of them, build a decision tree of max. depth 5. Calculate accuracy on validation set. **[2 marks]**

4. Carry out weighted classification of the test set using these 50 decision trees, along with their validation accuracies as weights. Report the accuracy. **[1 marks]**

5. Starting with this ensemble as the initial classifier, implement Adaboost algorithm. At each stage, build a decision tree using entropy based on weighted examples as the heterogeneity measure of each node. Each tree will have maximum depth of 5. Maximum 20 iterations of Adaboost. **[3 marks]**

6. Using this ensemble, carry out classification on the test set and report accuracy. **[1 mark]**
