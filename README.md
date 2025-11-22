# Car_Price_Prediction_Using_LinearRegression
A complete end-to-end Machine Learning project that predicts used car prices based on features like brand, model, manufacturing year, fuel type, and kilometers driven. This project includes data cleaning, feature engineering, EDA, model building using Scikit-Learn pipelines, and model persistence using Pickle.

This project uses the Quikr Car Dataset to build a regression model capable of estimating car prices.
The original data contains messy, unstructured columns (e.g., strings, missing values, mixed units), which are cleaned and transformed before modeling.

Key steps include:
Handling missing values
Data cleaning and preprocessing
Removing outliers
Exploratory Data Analysis (EDA)
Encoding categorical features
Building a Linear Regression + OneHotEncoder pipeline
Evaluating with R² score
Saving the final model as LinearRegressionModel.pkl

Data Cleaning & Preprocessing

The dataset required extensive cleaning:

Fixes Applied:
✔ Removed non-numeric year values
✔ Converted “Ask For Price” → removed
✔ Cleaned “kms_driven” by removing commas & text
✔ Dropped rows with null fuel types
✔ Extracted first 3 words of car names for uniformity
✔ Converted data types to integers
✔ Removed extreme outliers (cars priced > 60 Lakhs)

Exploratory Data Analysis (EDA)
Visualizations included:
Boxplots for price distribution
Swarmplot of Year vs Price
Relplot for KMs Driven vs Price
Company-wise price variation
Fuel-type vs price comparison
These helped identify patterns and outliers affecting prediction accuracy.

Model Performance

The best model achieved:

R² Score: ~0.845 After training the Hyperparameters

🛠 Tech Stack
Python
Pandas, NumPy
Matplotlib, Seaborn
Scikit-Learn
Pickle
