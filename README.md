
**Cab Fare Prediction Using Machine Learning**

**Overview**
This project aims to build a machine learning model that accurately predicts cab fares based on trip distance, time of day, passenger count, and other factors. By analyzing real-world cab data, the project explores various machine learning techniques to identify the most effective approach for fare prediction.

**Objectives**
1. **Fare Transparency**: Provide accurate and fair fare predictions to enhance customer satisfaction and reduce disputes.
2. **Model Optimization**: Compare and optimize multiple machine learning models to identify the best one for the task.
3. **Insight Generation**: Understand how factors like trip distance, pickup time, and passenger count influence cab fares.

---

**Key Features**
- **Data Cleaning and Preprocessing**: 
  - Filtered invalid or extreme values for fare amounts, passenger counts, and geographic coordinates.
  - Extracted time-related features (e.g., hour, day, month, year) from timestamps.
  - Calculated trip distances using geodesic coordinates.

- **Feature Engineering**:
  - Added new features like trip distance and temporal information to improve model performance.

- **Model Development and Evaluation**:
  - Implemented and compared multiple regression models, including:
    - Linear Regression
    - Decision Trees
    - Random Forest
    - Gradient Boosting
    - XGBoost
  - Used cross-validation and hyperparameter tuning to optimize models.

- **Hyperparameter Tuning**:
  - Used **RandomizedSearchCV** to find the best parameters for Gradient Boosting, improving accuracy and minimizing errors.

---

## **Technologies Used**
- **Programming Language**: Python
- **Libraries**:
  - **Data Processing**: `pandas`, `numpy`
  - **Visualization**: `matplotlib`, `seaborn`
  - **Machine Learning**: `scikit-learn`, `xgboost`
  - **Geospatial Calculations**: `geopy`

---
**Results**
- The best-performing model, **Gradient Boosting Regressor**, achieved:
  - **Mean Absolute Error (MAE)**: <2.1928612141312693>
  - **Root Mean Squared Error (RMSE)**: <4.691897328851626>
  - **R² Score**: <0.7676365166104603>
- Key insights:
  - Trip distance and pickup time significantly affect fare amounts.
  - Hyperparameter tuning improved model performance by reducing errors.

---

