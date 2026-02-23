
## 🔹 Scenario 1: Breast Cancer Classification using KNN

### Load Dataset

* Loaded Breast Cancer dataset into a Pandas DataFrame
* Displayed sample rows to verify data integrity

### Data Preparation

* Selected relevant numerical features
* Encoded target labels (Malignant / Benign)
* Performed Train–Test split
* Applied feature scaling using `StandardScaler`

### Model Training

* Implemented **K-Nearest Neighbors (KNN)** classifier
* Tested multiple values of **K**
* Trained model on scaled training data

### Model Evaluation

* Calculated Accuracy score
* Generated Confusion Matrix
* Produced Classification Report (Precision, Recall, F1-score)

### Visualization

* Plotted Accuracy vs K value
* Displayed decision boundary visualization
* Highlighted misclassified samples

---

## 🔹 Scenario 2: Loan Approval Prediction using Decision Tree

### Load Dataset

* Loaded Loan Prediction dataset
* Displayed dataset structure using `info()`

### Data Preprocessing

* Handled missing values
* Encoded categorical variables
* Split dataset into training and testing sets

### Model Training

* Implemented **Decision Tree Classifier**
* Compared shallow tree vs deep tree configurations
* Adjusted tree depth to study overfitting behavior

### Model Evaluation

* Computed Accuracy score
* Generated Confusion Matrix
* Produced detailed Classification Report

### Feature Analysis

* Extracted Feature Importance values
* Identified dominant factors influencing loan approval

### Visualization

* Decision tree structure visualization
* Feature importance bar chart
* Performance comparison plots
