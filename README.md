# Predicting-Credit-Card-Consumption-
This project aims to predict the **average credit card consumption for a leading bank's customers for the next three months. 
By analyzing customer demographics, behavioral data (assets/liabilities), and historical transaction patterns, the model identifies 
high-value spenders to help the bank optimize marketing strategies.


Dataset Description
The analysis integrates three primary data sources joined on `Customer ID`:
* **Customer Demographics:** Age, Income levels, Profession, and Banking tenure.
* **Customer Behavior:** 3-month history of Credit/Debit card spend, transaction counts, and active loan statuses.
* **Credit Consumption (Target):** The average spend for the following quarter (July - September).

Tech Stack
* **Language:** Python
* **Libraries:** Pandas, NumPy, Scikit-Learn
* **Model:** RandomForest Regressor
* **Optimization:** GridSearchCV for Hyperparameter tuning

Data Pipeline
1.  **Data Integration:** Merged Demographics, Behavior, and Consumption tables via inner joins.
2.  **Preprocessing:** * Numerical features scaled using `StandardScaler`.
    * Categorical features encoded via `OrdinalEncoder`.
    * Handled missing values in the target variable by separating them into a "Final Prediction" set.
3.  **Feature Selection:** Automated removal of low-variance (quasi-constant) features.
4.  **Modeling:** Implemented a Random Forest Regressor with Cross-Validation to minimize error.

Evaluation Metric
The model is evaluated using  RMSPE (Root Mean Square Percentage Error)**. This ensures that the error is relative to the actual spend, providing a more business-centric accuracy score.


   [click here] to  see the code 
