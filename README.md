# ml-assignment-
# California Housing Price Prediction

## Overview
This project analyzes the **California Housing Dataset** and builds regression models to predict **median house prices** based on various features such as location, income, and number of rooms. The project includes **data cleaning, preprocessing, exploratory data analysis (EDA), and multiple regression model evaluations.**

## Dataset
- **Source:** California Housing dataset
- **Number of Records:** 20,640
- **Features:** 10 (including numerical and categorical variables)
- **Target Variable:** `median_house_value` (House Price)

### Key Features:
- `longitude`, `latitude`: Geographical coordinates
- `housing_median_age`: Median age of the houses
- `total_rooms`, `total_bedrooms`, `households`, `population`: Housing-related counts
- `median_income`: Median household income in the area
- `ocean_proximity`: Categorical feature indicating the location relative to the ocean

## Data Preprocessing
- **Handling Missing Values:** `total_bedrooms` was imputed using the **median**.
- **Categorical Encoding:** One-hot encoding for `ocean_proximity`.
- **Feature Scaling:** Applied **StandardScaler** for numerical features.
- **Train-Test Split:** 80% Training, 20% Testing.

## Regression Models Used
1. **Linear Regression**
2. **Ridge Regression**
3. **Lasso Regression**
4. **Random Forest Regressor**
5. **Gradient Boosting Regressor**

## Model Performance
| Model               | MAE     | MSE         | R² Score |
|--------------------|---------|-------------|----------|
| Linear Regression | 50,670  | 4.91e+09    | 0.625    |
| Ridge Regression  | 50,668  | 4.91e+09    | 0.625    |
| Lasso Regression  | 50,670  | 4.91e+09    | 0.625    |
| Random Forest     | 31,631  | 2.40e+09    | 0.817    |
| Gradient Boosting | 38,248  | 3.12e+09    | 0.762    |

### Best Model: **Random Forest Regressor**
- **Achieved the highest R² Score (0.817)**
- **Lowest error rates (MAE & MSE)**



## Author
Developed by **[Abdulazeez Raheem]** 

## License
This project is open-source under the MIT License.

