# EX03 – Multilinear and Polynomial Regression using Scikit-Learn

---

## 📌 Experiment Title  
**EX03 – Multilinear Regression and Polynomial Regression**

## 🎯 Objective  
To understand and implement:
- **Multilinear Regression** for predicting student academic performance  
- **Polynomial Regression** for modeling non-linear relationships in real-world data  

using Python and **scikit-learn**.

---

## 🧰 Libraries Used
- `pandas` – data loading and preprocessing  
- `numpy` – numerical computations  
- `matplotlib`, `seaborn` – visualization  
- `scikit-learn` – preprocessing, modeling, regularization, and evaluation  

---

## 🔹 Scenario 1: Multilinear Regression – Student Performance Prediction

### Problem Statement  
Predict **student final exam performance** using multiple academic and socio-economic factors.

### Dataset  
- **Source:** Students Performance in Exams (Kaggle)  
- **File:** `StudentsPerformance.csv`

### Target Variable  
- **Final Exam Score**  
  - Computed as the average of:
    - Math score  
    - Reading score  
    - Writing score  

### Input Features  
- Gender  
- Race/Ethnicity  
- Parental level of education  
- Lunch type  
- Test preparation course  
- *(Simulated)* Study hours  
- *(Simulated)* Attendance percentage  
- *(Simulated)* Sleep hours  

### Steps Performed
- Loaded dataset into Pandas DataFrame  
- Created final score as target variable  
- Simulated missing behavioral features  
- Encoded categorical variables using **One-Hot Encoding**  
- Handled missing values using suitable imputation  
- Applied **StandardScaler** for feature scaling  
- Split data into training and testing sets  
- Trained **Multilinear Regression** model  
- Evaluated model using:
  - Mean Squared Error (MSE)  
  - Root Mean Squared Error (RMSE)  
  - R² Score  
- Analyzed regression coefficients  
- Applied **Ridge** and **Lasso** regression for regularization  

### Visualizations
- Predicted vs Actual final scores  
- Feature coefficient magnitude comparison  
- Residual distribution plot  

### Outcome
Academic support indicators such as test preparation and parental education showed strong influence. Regularization improved coefficient stability and reduced multicollinearity effects.

---

## 🔹 Scenario 2: Polynomial Regression – Auto MPG Prediction

### Problem Statement  
Predict **vehicle fuel efficiency (MPG)** based on **engine horsepower**, where the relationship is non-linear.

### Dataset  
- **Source:** Auto MPG Dataset (Kaggle / UCI)  
- **File:** `auto-mpg.csv`

### Target Variable  
- `mpg` – Miles per gallon  

### Input Feature  
- `horsepower`

### Steps Performed
- Loaded dataset and inspected data types  
- Converted horsepower from object to numeric  
- Handled missing values (`"?"`) using mean imputation  
- Selected horsepower as independent variable  
- Applied **StandardScaler**  
- Generated polynomial features of degrees 2, 3, and 4  
- Split dataset into training and testing sets  
- Trained polynomial regression models  
- Evaluated models using:
  - MSE  
  - RMSE  
  - R² Score  
- Compared performance across polynomial degrees  
- Applied **Ridge Regression** to reduce overfitting  

### Visualizations
- Polynomial curve fitting for different degrees  
- Training vs testing error comparison  
- Overfitting and underfitting demonstration  

### Outcome
Moderate-degree polynomial models captured non-linearity effectively. Higher-degree models showed overfitting, which was controlled using Ridge regularization.

---

## ✅ Key Learnings
- Importance of proper data cleaning and encoding  
- Role of feature scaling in regression models  
- Understanding non-linear relationships using polynomial features  
- Detecting and handling overfitting  
- Practical demonstration of the **bias–variance tradeoff**  
- Impact of regularization on model stability and generalization  

---

## 📌 Conclusion
This experiment demonstrates how regression techniques can be applied to both linear and non-linear problems, highlighting the importance of preprocessing, model selection, evaluation metrics, and regularization in real-world machine learning tasks.
