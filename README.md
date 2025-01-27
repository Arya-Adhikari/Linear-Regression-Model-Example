Predicting Monthly Bill based on Average Daily Usage

This project uses a simple linear regression model to predict the monthly bill based on the average daily usage of a product. The code demonstrates basic data processing, model training, evaluation, and visualization using Python's popular libraries: pandas, numpy, scikit-learn, matplotlib, and seaborn.

Libraries Used
pandas: For data manipulation and analysis.
numpy: For numerical operations.
scikit-learn: For machine learning functions, including linear regression and evaluation metrics.
matplotlib: For plotting graphs.
seaborn: For enhanced visualizations.

Dataset
The dataset used for this project contains two columns:

Average Daily Usage (hours): The number of hours a user typically uses the product daily.
Monthly Bill ($): The corresponding monthly bill based on the daily usage.

Example data:

Average Daily Usage (hours): [3, 4, 6, 7, 8, 10, 12]
Monthly Bill ($): [50, 60, 80, 95, 110, 130, 150]

Code Overview

1. Data Loading and Exploration

A simple dataset is created manually in the form of a dictionary and then converted to a pandas DataFrame.
The dataset is printed and analyzed to check its shape and basic statistics.
Missing values are checked using isnull().sum().

2. Data Preprocessing

The features (independent variables) and target (dependent variable) are selected.
The dataset is split into training and testing sets using train_test_split from scikit-learn.

3. Model Training

A Linear Regression model is initialized and trained on the training data using model.fit().

4. Model Evaluation

The model makes predictions on the test data.
Evaluation metrics like Root Mean Squared Error (RMSE) and R-squared score are calculated to assess the performance of the model.

5. Visualization

A scatterplot is created to visualize the relationship between the actual and predicted monthly bills.
A red diagonal line is plotted for reference, which represents perfect predictions.

6. Making Predictions

The model is used to predict the monthly bill for a given daily usage (e.g., 9 hours).

Key Functions and Metrics
Root Mean Squared Error (RMSE): Measures the average magnitude of errors between predicted and actual values.
R-squared Score: Represents the proportion of the variance for the dependent variable that is explained by the independent variable(s).

Mean Squared Error: 9.20
R-squared Score: 0.97

Predicted Monthly Bill for Average Daily Usage = 9 hours: $119.16
Visual Output
The code generates a plot comparing the actual vs predicted monthly bills. A red line indicates perfect predictions.

How to Run
Ensure that you have Python 3.x installed.

Install necessary libraries:

pip install pandas numpy scikit-learn matplotlib seaborn
Run the script to see the output and visualizations.
