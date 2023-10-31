# REAL  ESTATE PRICE FORECASTING USING REGRESSION MODELING

![Logo](https://assets.everspringpartners.com/dims4/default/3c5694c/2147483647/strip/true/crop/1400x800+0+0/resize/800x457!/format/webp/quality/90/?url=http%3A%2F%2Feverspring-brightspot.s3.us-east-1.amazonaws.com%2Ffe%2F06%2Ff23661be455e97d009c6ae418995%2Freal-estate-finance.jpg)

[![MIT License](https://img.shields.io/badge/License-MIT-green.svg)](https://choosealicense.com/licenses/mit/)
## Overview
The goal of this project is to develop a robust regression model for predicting house prices in a specific real estate market, thereby addressing the critical need for accurate and reliable property price estimations. 
By leveraging advanced data analysis techniques and predictive modeling, this initiative aims to provide invaluable insights to various stakeholders, including prospective homebuyers, sellers, real estate agents, and property investors.

## Installation and Setup
### Code and Resources Used
 - Editor: Google Colab (https://colab.research.google.com/)
-  Python version: Python 3.9
-  Code: student.ipynb
### Python Packages Used
- Data Manipulation: Pandas, Numpy
- Data Visualization: Matplotlib, Seaborn
- Regression Modeling: Sklearn, Statsmodels
  
## Repository Structure
├─ __pycache__

    ├─ functions.cpython-311.pyc
    
├─ data

     ├─ column_names.md
   
     ├─ kc_house_data.csv
   
├─ README.md

├─ functions.py

├─ student.ipynb

## Data
### Source Data
- King County House Sales Data (https://www.kaggle.com/datasets/harlfoxem/housesalesprediction?select=kc_house_data.csv)
### Features
- Categorical features: `id`, `date`, `bedrooms`,`bathrooms`, `floors`, `waterfront`, `view`, `grade`, `year_built`, `yr_renovated`, `zipcode`, `lat`, `long`.
- Numerical variables:`price`, `sqft_living`, `sqft_lot`, `sqft_above`, `sqft_basement`, `sqft_basement`, `sqft_living_above`, `sqft_lot_below`.
- Target variable: `price`
### Data Preprocessing
- No duplicates existed in the data.

- Found null values in some columns (`waterfront`, `view` and `yr_renovated`).

- Filled missing `waterfront` and `view` values based on mode of each per `zipcode`.

- Filled missing values in the `yr_renovated` column with **0**.
   
### Exploratory Data Analysis
- Explored relationships between price and other features
- Most features have a positive linear relationship with price
  
### Feature engineering
- Built new features: `age`, `total_sqft_house`,`average_price_by_zipcode`,`price_per_sqft`

### Regression Modeling
|Model|R-squared|RMSE|Observation|
|------|---------|--------|------------|
|Baseline Model| 46.01% | $124,066 | This model has weak predictive power |
|Multiple Linear regression model| 81.4% | $71,295 | High predictive power |

# Conclusion
- The multiple linear regression model is a good fit with a high R-squared value and low RMSE.
- Enhanced decision-making capabilities for stakeholders, facilitating more informed and data-driven business actions.
