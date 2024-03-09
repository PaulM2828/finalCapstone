# Simple Linear Regression Analysis

## Overview

This repository contains a Python script showcasing the application of simple linear regression, with a specific focus on exploring the relationship between age and BMI in the 'insurance.csv' dataset. The primary goal is to demonstrate the usage of machine learning tools from the scikit-learn library.

## Script Description

The provided Python script performs the following steps:

1. **Import Libraries:**

   Import essential libraries to facilitate data manipulation, visualization, and linear regression modeling:

   ```python
   import pandas as pd
   import matplotlib.pyplot as plt 
   from sklearn.linear_model import LinearRegression
   ```

2. **Load the Dataset:**

   Load the 'insurance.csv' dataset from the specified local path:

   ```python
   local_path = "/Users/paul/Desktop/python school/T18 - Supervised learning - Simple Linear Regression/insurance.csv"
   insurance_data = pd.read_csv(local_path)
   ```

   Display the first few rows of the dataset for initial exploration:

   ```python
   insurance_data.head()
   ```

3. **Explore Dataset Structure:**

   Check the structure of the dataset, including data types and missing values:

   ```python
   insurance_data.info()
   ```

4. **Summary Statistics:**

   Generate summary statistics to gain insights into the distribution of numerical variables:

   ```python
   insurance_data.describe()
   ```

5. **Visualize the Data:**

   Create a scatter plot to visually represent the relationship between age and BMI:

   ```python
   plt.figure(figsize=(12, 8))
   plt.scatter(insurance_data['age'], insurance_data['bmi'], alpha=0.8, color='green', label='Data Points')

   # Adding title and labels
   plt.title('Scatter Plot of Age vs BMI')
   plt.xlabel('Age')
   plt.ylabel('BMI')

   # Adding grid lines and legend
   plt.grid(True, linestyle='--', alpha=0.5)
   plt.legend()

   # Show the plot
   plt.show()
   ```

## Usage

1. **Clone the Repository:**

   Clone this repository to your local machine:

   ```bash
   git clone https://github.com/your-username/simple-linear-regression-analysis.git
   cd simple-linear-regression-analysis
   ```

2. **Run the Script:**

   Execute the Python script to perform simple linear regression analysis:

   ```bash
   python linear_regression_analysis.py
   ```

   Ensure to customize the `local_path` variable in the script to point to your 'insurance.csv' dataset.

3. **Explore the Results:**

   The script will provide visualizations and summary statistics to help you understand the relationship between age and BMI. Feel free to adapt the script for your specific use case or integrate it into your machine learning projects.

Feel free to customize and integrate this script into your workflow for simple linear regression analysis.