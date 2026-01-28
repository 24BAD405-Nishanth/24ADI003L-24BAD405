# EX02 – Regression and Classification using Scikit-Learn

---

## 🔹 Common Setup

### Libraries Used
- `pandas` – data loading and manipulation  
- `numpy` – numerical operations  
- `matplotlib`, `seaborn` – data visualization  
- `scikit-learn` – preprocessing, modeling, and evaluation  

---

## 🔹 Scenario 1: Ocean Water Temperature Prediction (Regression)

### Objective  
Predict **ocean water temperature (`T_degC`)** using environmental and depth-related features.

### Dataset  
- **Source:** CalCOFI Oceanographic Dataset (Kaggle)  
- **File Used:** `bottle.csv`

### Features Used
- `Depthm` – Depth in meters  
- `Salnty` – Salinity  
- `O2ml_L` – Dissolved oxygen  

### Target Variable
- `T_degC` – Water temperature (continuous)

### Steps Performed
- Loaded dataset into Pandas DataFrame  
- Selected relevant numerical features and target  
- Removed rows with missing target values  
- Imputed missing feature values using **median imputation**  
- Applied **StandardScaler** for feature scaling  
- Split data into training and testing sets  
- Trained models:
  - Linear Regression  
  - Ridge Regression  
  - Lasso Regression  
- Evaluated models using:
  - Mean Squared Error (MSE)  
  - Root Mean Squared Error (RMSE)  
  - R² Score  
- Visualized:
  - Actual vs Predicted temperature  
  - Residual error distribution  
- Compared performance before and after regularization  

### Outcome
Regularization improved model generalization, while depth emerged as the most influential predictor of ocean temperature.

---

## 🔹 Scenario 2: LIC Stock Price Movement Prediction (Classification)

### Objective  
Classify whether the **LIC stock price increased or decreased** on a given day.

### Dataset  
- **Source:** LIC Stock Price Dataset (Kaggle)  
- **File Used:** `LICI - Daily data.csv`

### Target Variable (Derived)
- `Price_Movement`
  - `1` → Closing price > Opening price  
  - `0` → Closing price ≤ Opening price  

### Features Used
- `Open` – Opening price  
- `High` – Highest price of the day  
- `Low` – Lowest price of the day  

*(Volume not available in daily data)*

### Steps Performed
- Loaded daily stock price data  
- Cleaned column names  
- Created binary target variable  
- Handled missing values using median imputation  
- Scaled features using **StandardScaler**  
- Split dataset into training and testing sets with stratification  
- Trained **Logistic Regression** model  
- Evaluated model using:
  - Accuracy  
  - Precision  
  - Recall  
  - F1-Score  
  - Confusion Matrix  
- Visualized:
  - Confusion Matrix heatmap  
  - ROC Curve  
  - Feature importance using model coefficients  
- Performed hyperparameter tuning using **GridSearchCV**  
- Compared baseline and optimized model performance  

### Outcome
Regularization improved classification stability, and price range features (`High`, `Low`) showed higher influence on daily price movement.

---

## 🔹 Conclusion

This experiment demonstrates:
- Proper handling of missing data  
- Importance of feature scaling  
- Use of regression for continuous prediction  
- Use of logistic regression for binary classification  
- Model evaluation using appropriate statistical metrics  