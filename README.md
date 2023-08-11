# Amazon_Product_Analysis

This project involves analyzing Amazon product data, exploring customer ratings, discounts, and other features, and performing linear regression analysis to predict discounted prices based on various factors.


Introduction:
The goal of this project is to analyze Amazon product data, understand the relationships between different variables, and predict discounted prices using linear regression techniques. We'll perform data preprocessing, visual exploratory analysis, and various linear regression methods to achieve this goal.

Data Preprocessing and Analysis:
We start by importing the necessary libraries and loading the Amazon product dataset. We check for missing values and duplicates, drop rows with null values, and convert data types to facilitate analysis. Columns like 'discounted_price' and 'actual_price' are cleaned and transformed to float data types. The 'rating' column is converted to a numeric format, and categorical features like 'sub_category' and 'main_category' are extracted from the 'category' column.

Exploratory Data Visualization
We use various visualizations to explore the dataset's characteristics:

Bar plots to visualize the most sold products by main and sub-categories.
Histograms to analyze the distribution of customer ratings, discount percentages, actual prices, and discounted prices.
Correlation matrix heatmap to understand the relationships between different numeric features.
Linear Regression
We perform linear regression analysis to predict discounted prices based on the 'actual_price' and other potential predictors. Three methods are used for linear regression:

Simple Linear Regression
We apply simple linear regression using 'actual_price' as the independent variable and 'discounted_price' as the dependent variable. We fit the model, calculate coefficients and intercept, and evaluate the R2 score and cross-validation results.

Lasso and Ridge Regression
Lasso and Ridge regression are applied with 'actual_price', 'rating', and 'rating_count' as predictors. We assess the performance of each model, including the determination of the alpha parameter and analysis of coefficients.

Linear Regression with Standard Scaler
The same predictors are used in linear regression, but this time the features are standardized using the StandardScaler. We evaluate the R2 score for this standardized model.

Conclusion:
This project provides insights into Amazon product data through exploratory data analysis and predictive modeling using linear regression techniques. By analyzing correlations and building regression models, we gain a better understanding of factors influencing product discounts and customer ratings.
