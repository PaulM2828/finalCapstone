# Simple Linear Regression Analysis

## Overview

This repository contains a Python script demonstrating the application of simple linear regression, focusing on the relationship between age and BMI in the 'insurance.csv' dataset. The primary objective is to showcase the usage of machine learning tools from the scikit-learn library.

## Requirements

Make sure you have the following libraries installed:

- pandas
- matplotlib
- scikit-learn

You can install them using:

```bash
pip install pandas matplotlib scikit-learn
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

   Make sure to customize the `local_path` variable in the script to point to your 'insurance.csv' dataset.

3. **Explore the Results:**

   The script will generate a scatter plot of age vs. BMI, allowing you to visually explore the relationship between these two variables. Additionally, it will print the linear regression equation representing the fitted model.

## Script Details

- **Import Libraries:**

   Ensure that the required libraries are imported at the beginning of your script:

   ```python
   import pandas as pd
   import matplotlib.pyplot as plt 
   from sklearn.linear_model import LinearRegression
   ```

- **Load the Dataset:**

   Load the 'insurance.csv' dataset from your local path:

   ```python
   local_path = "/path/to/your/dataset/insurance.csv"
   insurance_data = pd.read_csv(local_path)
   ```

- **Visualize the Data:**

   Plot a scatter plot to visually explore the relationship between age and BMI:

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

- **Perform Simple Linear Regression:**

   Use scikit-learn's LinearRegression to fit a regression model:

   ```python
   # Extract features and target variable
   X = insurance_data[['age']]
   y = insurance_data['bmi']

   # Initialize the linear regression model
   model = LinearRegression()

   # Fit the model to the data
   model.fit(X, y)

   # Access the coefficients
   slope = model.coef_[0]
   intercept = model.intercept_

   print(f"Linear Regression Equation: BMI = {slope:.2f} * Age + {intercept:.2f}")
   ```

   This step allows you to understand the linear relationship between age and BMI and obtain the equation of the regression line.

Feel free to customize and integrate this script into your workflow for simple linear regression analysis.