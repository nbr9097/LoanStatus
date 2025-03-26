
![Uploading Screenshot (455).png…]()

### Solution Description

The goal of this project is to automate the loan eligibility prediction for Dream Housing Finance using machine learning. Given customer data such as gender, marital status, income, loan amount, credit history, and property area, we predict if a loan will be approved (Y/N).

#### Steps Taken:

1. **Data Preprocessing**: 
   - Handled missing values by imputing median or mode values based on feature types.
   - Encoded categorical variables (Gender, Marital Status, etc.) into numerical form using label encoding and one-hot encoding.
   - Combined ApplicantIncome and CoapplicantIncome into TotalIncome for better predictive power.
   - Scaled numerical features to improve model stability.

2. **Model Selection**:
   - Tested multiple algorithms, including Logistic Regression, Decision Tree, Random Forest, and Gradient Boosting.
   - Tuned hyperparameters of the Random Forest model using GridSearchCV, resulting in the best parameter combination: `{'max_depth': 20, 'min_samples_leaf': 2, 'min_samples_split': 2, 'n_estimators': 50}` with an accuracy of 82.27%.

3. **Final Model & Prediction**:
   - The optimized Random Forest model was trained on the full training dataset and used to predict loan eligibility on the test dataset.
   - Results were saved in `loan_eligibility_submission.csv`, meeting the required format (Loan_ID, Loan_Status).

#### Future Improvements:
Potential improvements include advanced ensemble techniques, further feature engineering (e.g., income-to-loan ratios), and experimenting with other models like XGBoost.

---

This description gives a clear overview of the process, methods, and improvements made to increase the model's performance. Let me know if you’d like to add any further details!
### Solution Description

The goal of this project is to automate the loan eligibility prediction for Dream Housing Finance using machine learning. Given customer data such as gender, marital status, income, loan amount, credit history, and property area, we predict if a loan will be approved (Y/N).

#### Steps Taken:

1. **Data Preprocessing**: 
   - Handled missing values by imputing median or mode values based on feature types.
   - Encoded categorical variables (Gender, Marital Status, etc.) into numerical form using label encoding and one-hot encoding.
   - Combined ApplicantIncome and CoapplicantIncome into TotalIncome for better predictive power.
   - Scaled numerical features to improve model stability.

2. **Model Selection**:
   - Tested multiple algorithms, including Logistic Regression, Decision Tree, Random Forest, and Gradient Boosting.
   - Tuned hyperparameters of the Random Forest model using GridSearchCV, resulting in the best parameter combination: `{'max_depth': 20, 'min_samples_leaf': 2, 'min_samples_split': 2, 'n_estimators': 50}` with an accuracy of 82.27%.

3. **Final Model & Prediction**:
   - The optimized Random Forest model was trained on the full training dataset and used to predict loan eligibility on the test dataset.
   - Results were saved in `loan_eligibility_submission.csv`, meeting the required format (Loan_ID, Loan_Status).

#### Future Improvements:
Potential improvements include advanced ensemble techniques, further feature engineering (e.g., income-to-loan ratios), and experimenting with other models like XGBoost.
