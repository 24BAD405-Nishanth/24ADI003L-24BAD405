# EX04 – Naive Bayes Classifier using Scikit-Learn

---

## 📌 Experiment Title  
**EX04 – Naive Bayes Classifier**

## 🎯 Objective  
To understand and implement:  
- **Multinomial Naive Bayes** for text classification in spam detection  
- **Gaussian Naive Bayes** for tabular data classification in species prediction  

using Python and **scikit-learn**.

---

## 🧰 Libraries Used
- `pandas` – data loading and preprocessing  
- `numpy` – numerical computations  
- `matplotlib`, `seaborn` – visualization  
- `nltk` – text preprocessing (stopwords, tokenization)  
- `scikit-learn` – preprocessing, modeling, and evaluation  

---

## 🔹 Scenario 1: Multinomial Naive Bayes – SMS Spam Detection

### Problem Statement  
Classify SMS messages as **spam** or **ham** based on message content.

### Dataset  
- **Source:** SMS Spam Collection (UCI)  
- **File:** `spam.csv`

### Target Variable  
- `label` – Spam (1) or Ham (0)  

### Input Features  
- `message` – Raw text of the SMS  

### Steps Performed
- Loaded dataset into Pandas DataFrame  
- Performed text preprocessing: lowercase, punctuation removal, stopword removal  
- Encoded labels using **LabelEncoder**  
- Vectorized text using **TF-IDF Vectorizer**  
- Split data into training and testing sets  
- Trained **Multinomial Naive Bayes** model  
- Evaluated model using:  
  - Accuracy Score  
  - Precision Score  
  - Recall Score  
  - F1 Score  
  - Confusion Matrix  
  - Classification Report  
- Analyzed misclassified examples  
- Extracted top words influencing spam/ham classification  

### Visualizations
- Word clouds for spam and ham messages  
- Confusion matrix heatmap  
- Top 20 words in spam and ham messages (bar plots)  

### Outcome
The model achieved high accuracy in detecting spam, with keywords like "free", "claim", and "prize" strongly influencing spam predictions. Misclassified examples often contained ambiguous phrasing.

---

## 🔹 Scenario 2: Gaussian Naive Bayes – Iris Species Classification

### Problem Statement  
Classify **iris flowers** into species based on sepal and petal measurements.

### Dataset  
- **Source:** Iris Dataset (scikit-learn / UCI)  
- **Loaded via:** `load_iris()`

### Target Variable  
- `species` – Setosa (0), Versicolor (1), Virginica (2)  

### Input Features  
- Sepal length  
- Sepal width  
- Petal length  
- Petal width  

### Steps Performed
- Loaded dataset and converted to Pandas DataFrame  
- Inspected data for missing values and statistics  
- Applied **StandardScaler** for feature scaling  
- Split data into training and testing sets  
- Trained **Gaussian Naive Bayes** model  
- Evaluated model using:  
  - Accuracy Score  
  - Classification Report  
  - Confusion Matrix  
- Compared performance with **Logistic Regression**  

### Visualizations
- Pairplot of features by species  
- Confusion matrix heatmap  
- Decision boundary plot (using sepal features)  

### Outcome
The model classified species with perfect accuracy on the test set, performing as well as Logistic Regression. Gaussian NB effectively handled the continuous features and class separations.