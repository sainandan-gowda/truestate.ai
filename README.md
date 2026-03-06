# Real Estate Price Prediction (Price per Square Meter)

## Project Overview
This project builds a Proof-of-Concept regression model to predict **property price per square meter** using real estate transaction data.

The dataset contains property details such as:
- Property type
- Location information (Area, Project, Landmarks)
- Nearby amenities (Metro, Mall, Parking)
- Transaction details and dates

## Objective
Predict the **meter_sale_price** using machine learning techniques.

---

## Workflow

### 1. Data Cleaning
- Handled missing values
- Converted date features
- Grouped rare categorical values
- Encoded categorical variables

### 2. Feature Engineering
- Extracted **year and month from transaction date**
- Processed **location-based features**
- Encoded categorical variables using:
  - Target Encoding
  - One-Hot Encoding

### 3. Model
Used **Gradient Boosting Regressor** because it performs well on structured/tabular datasets and can capture complex non-linear relationships between features. 
Gradient boosting builds an ensemble of decision trees sequentially, where each new tree attempts to correct the errors made by the previous trees. 
This helps improve prediction accuracy while reducing bias.

### 4. Evaluation Metrics
The model was evaluated using:

- MAE (Mean Absolute Error) : 1703.43
- RMSE (Root Mean Squared Error) : 56176.98
- R² Score : 0.78

