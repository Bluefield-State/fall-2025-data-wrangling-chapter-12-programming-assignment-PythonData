# Chapter 12 Programming Assignment

## Problem Statement

You are provided with a CSV file named `housing_data.csv` that contains information about housing prices. Your tasks are to load the data, preprocess it, build a linear regression model, and evaluate its performance.

**CSV File: `housing_data.csv`**

| Column Name   | Description                                                   |
|---------------|---------------------------------------------------------------|
| `square_feet` | Size of the house in square feet.                             |
| `num_bedrooms`| Number of bedrooms in the house.                              |
| `num_bathrooms`| Number of bathrooms in the house.                            |
| `age`         | Age of the house in years.                                   |
| `price`       | Sale price of the house.                                     |

### Tasks

1. **Read the Data:**
   - Load the `housing_data.csv` file into a pandas DataFrame.

2. **Data Preprocessing:**
   - Check for and handle any missing values in the dataset.
   - Create dummy variables for any categorical features if present (not applicable in this dataset but good practice).

3. **Split the Data:**
   - Split the dataset into training and testing sets (80% train, 20% test).

4. **Build a Linear Regression Model:**
   - Use `statsmodels` to create a linear regression model predicting `price` based on `square_feet`, `num_bedrooms`, `num_bathrooms`, and `age`.
   - Include an intercept in the model.

5. **Evaluate the Model:**
   - Print the model summary to evaluate the coefficients and statistical significance.
   - Predict house prices on the test set and calculate the mean absolute error (MAE) of the predictions using `scikit-learn`.

6. **Output the Results:**
   - Print the MAE of the model.

## Expected Output

After running the notebook, the output should include:

1. A summary of the linear regression model, showing coefficients, standard errors, and statistical significance.
2. The Mean Absolute Error (MAE) of the model predictions on the test set, which indicates how well the model performs.