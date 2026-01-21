
## 🔹 Common Setup

### Importing Libraries
- Imported `pandas` for data handling
- Imported `matplotlib.pyplot` and `seaborn` for visualization

---

## 🔹 Scenario 1: Sales Data Analysis

### Load Dataset
- Read the CSV file into a Pandas DataFrame
- Displayed the dataset to verify correct loading

### Data Exploration
- Viewed first and last rows
- Checked dataset structure using `info()`
- Generated summary statistics using `describe()`

### Feature Creation
- Created a new column `Sales`
- Formula used:
  ```
  Sales = Quantity * UnitPrice
  ```

### Data Aggregation
- Grouped data by product identifier
- Calculated total sales for each product

### Visualization
- Generated a bar chart for top-selling products
- Generated a line chart to show sales trends

---

## 🔹 Scenario 2: Diabetes Dataset Analysis

### Load Dataset
- Loaded diabetes CSV file
- Displayed the DataFrame

### Data Validation
- Checked for missing values in each column

### Distribution Analysis
- Created histogram for glucose levels
- Created histogram for age distribution

### Outlier Detection
- Used boxplots to detect outliers in:
  - Glucose values
  - Age values

---

## 🔹 Scenario 3: Housing Data Analysis

### Load Dataset
- Loaded housing dataset
- Displayed sample rows and dataset information

### Relationship Analysis
- Created scatter plot for Area vs Price
- Created scatter plot for Bedrooms vs Price with furnishing status

### Correlation Analysis
- Selected numerical columns
- Computed correlation matrix
- Visualized correlations using heatmap

---

## 🔹 Scenario 4: Marketing Campaign Analysis

### Load Dataset
- Loaded marketing campaign dataset
- Checked dataset info and missing values

### Feature Engineering
- Created `Age` column using year of birth
- Created `Total_Spending` by summing all purchase columns

### Group Analysis
- Calculated average spending by education level

### Visualization
- Bar chart for education vs spending
- Boxplot for income distribution
- Boxplot for age vs campaign response

---