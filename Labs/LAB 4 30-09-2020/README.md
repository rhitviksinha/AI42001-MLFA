# LAB 4

## Wednesday, 30<sup>th</sup> September, 2 - 5 PM

# Assignment 4

The third assignment is **Daily Rainfall Analysis** using a **Linear Regression**, **Lasso Regression** and **Decision Tree Regression**.

### Datasets

1. [2010rainfall.mat](./datasets/2010rainfall.mat)

2. [2011rainfall.mat](./datasets/2011rainfall.mat)

### Description:

Two files are attached which contain daily rainfall data over India for 2010 and 2011. Both of them contain a 357x122 matrix (`XR1` and `XR`) an a binary vector (`ZR1` and `ZR`). The matrices contain rainfall amounts at `357` locations over India, on each day during the monsoon seasons of 2010 and 2011 (`122` days from 1 June to 30 September). `ZR1` and `ZR` are binary vectors which classify every day as "rainy" (`1`) or "non-rainy" (`0`) based on the rainfall across the landmass.

1. Read the .mat files in Python and access the variables

2. Use a linear regression model to predict the rainfall `XR(s,t)` at any location `s` on day `t`, using as predictor the rainfall at all other locations on the same day, and also rainfall at the same location on the previous 2 days `[XR(1,t)....XR(s-1,t), XR(s+1,t),....XR(357,t), XR(s,t-1), XR(s,t-2)]`. Use 2010 data for training.
  
  Build such a model for `s=42` (Mumbai), `s=158` (Delhi), `s= 299` (Kharagpur) **[3 marks]**

3. Use the same model to predict the rainfall at these 3 locations on each day of 2011.  Use values in XR as predictors. Compare the results with the true values and compute error for 3 locations separately. **[1 marks]**

4. Repeat the same process using LASSO linear regression. Using the coefficients, identify the top 5 predictors for each of the 3 locations. **[2 marks]**

5. Use Decision Tree on 2010 data to classify each day as `1` or `0` (as given in `ZR1`). For each day, use the 357-dimensional rainfall vector as feature vector. Report the 10 most discriminative features (i.e. locations) **[3 marks]**

6. Use this Decision Tree to classify each day of 2011 as `1` or `0`. Report accuracy by comparing with `ZR`. **[1 mark]**
