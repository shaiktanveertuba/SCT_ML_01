##Task 01 — House Price Prediction Using Linear Regression
##Objective:
Build a Linear Regression model to predict house prices based on square footage, 
number of bedrooms, and number of bathrooms.

What is Linear Regression?
Linear Regression is a supervised machine learning algorithm that establishes a relationship 
between input features and a continuous output variable by finding the best-fit line. It learns coefficients 
for each feature that minimize prediction error.

formula:
Price = (w1 × sqft) + (w2 × bedrooms) + (w3 × bathrooms) + bias

Dataset
1000 house records with features: sqft_living, bedrooms, bathrooms, and price as the target variable.
Steps Followed
1. Data Preparation — Loaded and explored dataset using descriptive statistics.
2. Feature Selection — Selected sqft_living, bedrooms, bathrooms as inputs.
3. Train-Test Split — 80% training, 20% testing using train_test_split.
4. Model Training — Trained LinearRegression from scikit-learn.
5. Evaluation — Measured MAE, RMSE, and R² on test data.

Results
Metric       Value
MAE          $15,741 
RMSE         $20,027 
R²Score      0.9152 (91.52%)

Model Coefficients
Feature          Impact
Square Footage   +$49.68 per sqft
Bedrooms         +$14,688 per bedroom
Bathrooms        +$11,836 per bathroom
Base Price       $54,043

Visualizations:
Actual vs Predicted prices scatter plot
Residual plot to check error distribution
Price vs Square Footage colored by bedrooms
Feature coefficients bar chart

Libraries Used
pandas, numpy, scikit-learn, matplotlib, seaborn

Conclusion
The model achieved an R² of 91.52%, explaining over 91% of variance in house prices. Coefficients align with real-world intuition — larger homes with more rooms cost more. This task demonstrates the complete ML pipeline from data prep to evaluation.
