# PRODIGY_ML_01
# Linear Regression Project

This repository contains files related to a linear regression project under my ML internship at Prodigy InfoTech. The project is divided into two main files, each serving a specific purpose. Here's a brief overview of each file:

## File 1: Data.ipynb

### Description
This Jupyter Notebook file focuses on data preprocessing and analysis. It prepares the dataset for building a linear regression model.

### Steps:
1. Imported the 'Houseprice' dataset.
2. Dropped irrelevant columns and checked for zero values in the dataset. Converted 0 values to NaN and determined whether the zero value makes sense for the column or not.
3. Imputed the zero values based on the distribution of the column.
4. Rounded the decimal points in the dataset.
5. Converted the "sqft_basement" and "yr_renovated" columns into binary columns and renamed them.
6. Conducted statistical analysis on the dataset columns.
7. Addressed outliers in the columns based on the "Winsorization" technique and addressed skewness using the "Box-Cox" technique.
8. Saved the modified data into a file named "After_Modifications.csv".

## File 2: LRModel.ipynb

### Description
This Jupyter Notebook file is focused on building and evaluating a linear regression model. It uses the modified dataset prepared in 'Data.ipynb'.

### Steps:
1. Import the modified data from 'After_Modifications.csv'.
2. Split the data into training and testing sets for model evaluation.
3. Build a linear regression model and evaluate its performance.
4. Use Recursive Feature Elimination (RFE) to select the top 5 features and build a new linear regression model with these features.
5. Attempt Lasso regression and cross-validation techniques to increase the model's accuracy.

