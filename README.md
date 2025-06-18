# Customer-Retention-Analytics
Customer Retention Analytics predicts churn using refined features through scaling and selection, enabling accurate, high-impact insights via XGBoost to drive proactive retention strategies.

# Customer Retention Analytics

A machine learning project to predict customer churn using real-world telecom data. The pipeline integrates effective feature engineering, feature scaling, and XGBoost to identify customers likely to leave, helping businesses improve retention strategies.

## Dataset Overview

The dataset contains anonymized customer data with 21 columns and includes behavioral, demographic, and billing information.

**Key Columns**:
- `customerID`: Unique identifier
- `gender`, `SeniorCitizen`, `Partner`, `Dependents`: Demographics
- `tenure`, `MonthlyCharges`, `TotalCharges`: Customer value metrics
- `Contract`, `InternetService`, `PaymentMethod`: Service types
- `Churn`: Target variable (Yes/No)

**Sample Record**:
| customerID | gender | SeniorCitizen | Partner | Dependents | tenure | PhoneService | InternetService | MonthlyCharges | TotalCharges | Churn  |
|------------|--------|---------------|---------|------------|--------|--------------|-----------------|----------------|--------------|--------|
| 7590-VHVEG | Female | 0             | Yes     | No         | 1      | No           | DSL             | 29.85          | 29.85        | No     |

---

## Pipeline Highlights

-  **Data Cleaning**: Handled missing/invalid values in `TotalCharges`.
-  **Encoding**: Applied Label to categorical features.
-  **Scaling**: Normalized numerical features using `StandardScaler`.
-  **Feature Selection**: Selected top k-features using `SelectKBest (chi2)`.
-  **Model**: XGBoost Classifier trained and validated on processed data.
-  **Evaluation**: Accuracy

---

