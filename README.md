# NY House Price Prediction (Linear Regression)

## Overview
This project predicts NY house prices using a linear regression model trained on cleaned and transformed property data.  
It demonstrates end-to-end preprocessing - handling missing values, log transformations, winsorisation, categorical encoding, and data leakage prevention.

## Process Summary
- Explored and profiled the dataset to identify missing values and outliers. 
- Cleaned inconsistent entries (addresses, placeholder square footage values).
- Split the data into training and test sets before any learned transformations.  
- Applied log transformations and winsorisation to normalise skewed variables.  
- Grouped rare categorical values and used target encoding on key features. 
- Standardised numerical features and trained a linear regression model.  
- Evaluated performance on the test set using MAE, MSE, and R² metrics.  

## Results
- **R² (Train):** 0.72  
- **R² (Test):** 0.70  
- **MAE:** 0.39  
- **MSE:** 0.28  
- Property square footage, number of bathrooms, and location exert the strongest influence on house price, while the number of bedrooms and property type have a noticeably weaker effect.

## Key Learnings
- Always perform data train/test splits before transformations that compute dataset statistics to avoid leakage.
- Log transformations stabilise variance and improve model fit.

## Requirements
- Python 3.10+  
- pandas, numpy, scikit-learn, matplotlib, seaborn, scipy, math
