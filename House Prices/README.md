# Predicting House Prices

## Description
This project is focused on building a predictive model to estimate house prices using the Boston Housing Dataset. The dataset contains various features of houses and their respective prices, and the goal is to explore the data, preprocess it, and build an efficient machine learning model.

## This repository includes:

1. Data exploration: 
    Understanding the dataset through visualization and statistical analysis.
2. Data preprocessing: 
    Handling missing values, univariate and bovaroate analysis, scaling, and splitting data into training and testing sets.
3. Model building: 
    Implementing regression models to predict house prices.
4. Hyperparameter Tuning: 
    Optimization of model performance using Grid Search and Randomized Search.
5. Evaluation: 
    Assessing the performance of the model using metrics like Mean Squared Error (MSE) and R-squared.


## Dataset
The Boston Housing Dataset includes:

  Features: Crime rate, zoning, industrial proportion, etc.
  Target: Median value of owner-occupied homes in $1000s.

  Can found the dataset in the main folder


## Exploratory Data Analysis (EDA)
The following steps were performed to understand the dataset:

1. Statistical Summary:
    Descriptive statistics for each feature.
    Identification of missing values and data types.

2. Visualization:
    Correlation heatmap to identify relationships between features.
    Distribution plots for individual features.
    Scatter plots to explore relationships between key features and the target variable (medv aka price).

3. Outlier Analysis:
    Boxplots to identify outliers in numerical features.
    Removal or transformation of extreme values for better model performance.


## Model Building and Tuning

1. Models Implemented
  
    Baseline Model: Linear Regression for initial predictions.

    Regularized Models: Ridge and Lasso Regression to address multicollinearity.

    Tree-Based Models: Decision Trees and Random Forests for handling non-linear relationships.


2. Hyperparameter Tuning

    Grid Search and Randomized Search were used to optimize hyperparameters for models:

    a. Ridge and Lasso: alpha (regularization strength)

    b. Random Forest: n_estimators, max_depth, min_samples_split, and min_samples_leaf.


## Evaluation
The models were evaluated using the following metrics:

1. Mean Squared Error (MSE): Measures the average squared difference between predicted and actual values.

2. R-squared Score: Indicates the proportion of variance explained by the model.


## Results

The performance metrics for various models are summarized below:

  ![Results](image-3.png)


## Conclusion

1. Polynomial Regression achieved the best overall performance with the lowest RMSE (2.327) and the highest R² (0.916), making it the most suitable model for this dataset.

2. Random Forest Regressor also delivered strong performance, with the original configuration slightly outperforming the hyperparameter-tuned version in this case.

3. Linear Regression provided decent results but was surpassed by more complex models like Polynomial Regression and Random Forest.

4. Ridge Regression performed the weakest, likely due to the limitations of regularization for this dataset.

5. Log-Transformed Target Variable improved over Linear Regression but still did not match the performance of Polynomial Regression or Random Forest.


## Recommendation: 

  1. Polynomial Regression is the best-performing model for this dataset, capturing non-linear relationships effectively.
  
  2. For scenarios requiring model robustness and scalability, Random Forest (with its best hyperparameters) is a competitive alternative.



