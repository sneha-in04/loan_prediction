# loan_prediction
# 🏦 Loan Approval Prediction System

A machine learning-based system that predicts whether a loan application will be approved or rejected, based on applicant details such as income, credit history, education, and more. The model is deployed using a Streamlit web app to allow real-time user input and loan decision feedback with probability scores.

---

## 📌 Features

- Uses Random Forest (with GridSearchCV) for robust classification
- Includes engineered features like:
  - `TotalIncome`: Applicant + Coapplicant income
  - `Income_to_Loan_Ratio`: Ratio of total income to loan amount
----
## 📊 Model Performance
LogisticRegression accuracy: 0.758
RandomForest accuracy: 0.790
GradientBoosting accuracy: 0.790
XGBoost accuracy: 0.742
##Final Model: Random Forest with GridSearchCV

We used a Random Forest Classifier with hyperparameter tuning via GridSearchCV to predict loan approval decisions. The best-performing model achieved a cross-validated accuracy of **81.27%**.

### Final Evaluation Metrics on Test Data
- **ROC-AUC Score**: 0.8693
- **Precision**: 83.9%
- **Recall**: 100.0%
- **F1-Score**: 89.13%

The high recall indicates that the model successfully identified all approved loans, while the solid F1-score shows a strong balance between precision and recall.
##  ROC Curve Analysis

The ROC Curve illustrates the trade-off between the true positive rate and false positive rate of our classifier.  model achieved an AUC  of **0.87**, indicating **excellent classification**.

- **True Positive Rate (TPR)**: High, showing that the model correctly identifies positive cases (e.g., approved loans).
- **False Positive Rate (FPR)**: Low, indicating that it makes few incorrect positive predictions.
- The curve's steep ascent toward the top-left shows that the model is both **sensitive and specific**, making it highly reliable.

This further validates that our Random Forest model is effective in making accurate predictions on unseen loan application data.


