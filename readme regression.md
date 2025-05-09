Coffee Shop Revenue Prediction

This project uses **machine learning regression techniques** to predict a coffee shop’s **daily revenue** based on several business indicators such as customer count, average order value, marketing spend, and more. It follows an end-to-end data science pipeline including data cleaning, exploratory analysis, feature engineering, and model evaluation


Project Objective

To build an accurate regression model that predicts **Daily Revenue** for a coffee shop using operational features such as:

- Number of Customers Per Day  
- Average Order Value  
- Marketing Spend Per Day  
- Location Foot Traffic  
- Operating Hours Per Day  
- Number of Employees

Dataset

- Source: coffee_shop_revenue.csv (local dataset)
- Size: ~1,750 records
- Features:
  - Continuous: `Number_of_Customers_Per_Day`, `Average_Order_Value`, `Marketing_Spend_Per_Day`, `Location_Foot_Traffic`, `Daily_Revenue`
  - Discrete: `Operating_Hours_Per_Day`, `Number_of_Employees`

 Workflow Summary

 1. Data Exploration & Cleaning
- Removed a row with negative daily revenue
- Handled duplicates and verified data types
- Identified skewed distributions and outliers

 2. Exploratory Data Analysis (EDA)
- Visualized distributions and relationships via:
  - Boxplots for outliers
  - Correlation matrix to identify influential predictors

3. Regression Modeling
- Used **OLS Regression** to calculate **Variance Inflation Factor (VIF)** and check multicollinearity
- Applied **Random Forest Regressor** for final prediction

 4. Model Evaluation
- Evaluated performance using:
  - R² Score
  - Mean Squared Error (MSE)
  - Mean Absolute Error (MAE)

Technologies Used

- Languages & Tools: Python, Jupyter Notebook
- Libraries:
  - `pandas`, `numpy` — Data handling
  - `matplotlib`, `seaborn` — Visualization
  - `sklearn`, `statsmodels` — Modeling and statistics

 Key Insights

- Marketing Spend and Foot Traffic are strong predictors of revenue.
- Reducing outliers significantly improved model performance.
- VIF helped in eliminating multicollinearity for better generalization.


License

This project is licensed under the **MIT License**.



Model Results Summary

The regression model was successfully trained to predict daily revenue for a coffee shop using multiple operational features. After evaluating different models, the Random Forest Regressor provided the best performance.

Final Evaluation Metrics:

R² Score: 0.89
Indicates that 89% of the variance in revenue is explained by the model.

VALIDATION: 0.86

The model performs well on unseen test data and can be considered a reliable tool for predicting revenue based on input features like customer count, order value, and marketing spend.

The model can predict the future daily sales so the company can plan accordingly








