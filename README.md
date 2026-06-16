# Automobile Data Wrangling Project

## Overview
This project focuses on data wrangling and preprocessing using the UCI Automobile dataset. The goal is to clean raw data and transform it into a structured format suitable for analysis and machine learning.

## Dataset
The dataset is sourced from the UCI Machine Learning Repository:
Automobile Data Set (imports-85). You can find the dataset [here.](https://archive.ics.uci.edu/ml/machine-learning-databases/autos/imports-85.data)

It contains information about different car models including specifications, fuel type, engine features, and pricing.

## Objectives
- Handle missing values and inconsistent data entries
- Convert data types to appropriate formats
- Perform feature engineering and normalization
- Create new features (e.g., fuel consumption in L/100km)
- Encode categorical variables using one-hot encoding
- Prepare dataset for modeling

## Key Data Wrangling Steps

### 1. Data Cleaning
- Replaced missing values represented as "?" with NaN
- Filled missing numeric values using mean imputation
- Filled categorical missing values using mode
- Dropped rows with missing target values (price)

### 2. Feature Engineering
- Converted:
  - `city-mpg` → `city-L/100km`
  - `highway-mpg` → `highway-L/100km`
- Normalized dimensions: `length`, `width`, `height`

### 3. Data Transformation
- Converted data types (e.g., horsepower → integer)
- Binned horsepower into categories (Low, Medium, High)

### 4. Encoding Categorical Variables
- Applied one-hot encoding to:
  - `fuel_type`
  - `aspiration`

### 5. Final Output
- Cleaned dataset exported as `clean_df.csv`

## Tools Used
- Python
- Pandas
- NumPy
- Matplotlib

## Files in Repository
- `data_wrangling.ipynb` → Jupyter Notebook containing full workflow
- `clean_df.csv` → Final cleaned dataset
- `README.md` → Project documentation

## Author
[Mohammed Ganiyu](www.linkedin.com/in/mohammed-ganiyu-930529405)
