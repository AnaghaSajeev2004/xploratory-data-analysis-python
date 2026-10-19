# Exploratory Data Analysis (EDA) Using Python 📊



This repository contains my hands-on practice in **Exploratory Data Analysis (EDA)** using Python. The notebook explores the Titanic dataset to understand its structure, identify missing and duplicate values, analyze passenger survival patterns, and visualize relationships between different variables.

It also covers essential data preprocessing techniques, including feature scaling and categorical variable encoding using Scikit-learn.

This project is part of my learning journey in Data Analytics and Machine Learning.

## 🎯 Objectives

- Explore and understand a dataset using Python.
- Inspect dataset structure, data types, and summary statistics.
- Identify duplicate records and missing values.
- Visualize passenger survival patterns and age distributions.
- Analyze correlations between numerical variables.
- Apply standardization and normalization techniques.
- Convert categorical variables into numerical representations.

## 🛠️ Technologies and Libraries Used

- **Python** – Programming language
- **Pandas** – Data manipulation and analysis
- **NumPy** – Numerical computing
- **Matplotlib** – Data visualization
- **Seaborn** – Statistical visualization
- **Scikit-learn** – Data preprocessing and encoding
- **Jupyter Notebook** – Interactive coding environment

## 📂 Project Contents

The notebook covers the following topics:

### 1. Dataset Exploration
- Loading the Titanic dataset using Seaborn
- Checking dataset shape and size
- Inspecting column names and data types
- Using `head()`, `tail()`, `info()`, and `describe()`

### 2. Data Cleaning
- Identifying duplicate records
- Removing duplicate records
- Detecting missing values using `isnull()`
- Checking the number of missing values in each column

### 3. Data Visualization
- Passenger survival count
- Passenger gender distribution
- Survival comparison by gender
- Survival comparison by passenger class
- Age distribution using histograms and KDE
- Age comparison across passenger classes using box plots

### 4. Correlation Analysis
- Selecting numerical columns
- Calculating correlation coefficients
- Creating a correlation heatmap
- Exploring relationships between numerical variables using pair plots

### 5. Feature Scaling
Using Scikit-learn to transform numerical features such as age and fare.

- `StandardScaler` – Standardization
- `MinMaxScaler` – Normalization to a specified range
- Comparing original and scaled values

### 6. Categorical Variable Encoding
Converting categorical data into numerical form for machine learning.

- One-hot encoding using `pd.get_dummies()`
- Combining encoded columns with the original dataset
- Understanding the dummy variable trap
- Label encoding using `LabelEncoder`
- One-hot encoding using `OneHotEncoder`
- Applying `ColumnTransformer`

## 💻 Sample Code

```python
import pandas as pd
import seaborn as sns
import matplotlib.pyplot as plt

# Load the Titanic dataset
df = sns.load_dataset("titanic")

# Explore the dataset
print("Dataset Shape:", df.shape)
print("\nData Types:")
print(df.dtypes)

print("\nMissing Values:")
print(df.isnull().sum())

# Visualize passenger survival
sns.countplot(data=df, x="survived")
plt.title("Titanic Passenger Survival Count")
plt.xlabel("Survived (0 = No, 1 = Yes)")
plt.ylabel("Number of Passengers")
plt.show()
```

## ▶️ How to Run the Notebook

1. Clone or download this repository.
2. Install Python on your computer.
3. Install the required libraries:

   ```bash
   pip install pandas numpy seaborn matplotlib scikit-learn notebook
   ```

4. Start Jupyter Notebook:

   ```bash
   jupyter notebook
   ```



**Note:** The later encoding examples use a CSV file named `homeprices (1).csv`. Make sure this file is available at the path specified in the notebook, or update the file path to match your local setup.

## 🎓 Learning Outcomes

Through this project, I am developing practical skills in:

- Exploratory data analysis
- Data cleaning and missing-value inspection
- Statistical data visualization
- Correlation analysis
- Feature scaling and normalization
- Categorical data encoding
- Preparing datasets for machine learning

## 🚀 Future Improvements

- Perform deeper analysis of Titanic passenger survival factors.
- Explore additional datasets from real-world applications.
- Apply further data cleaning and feature engineering techniques.
- Build machine learning models using prepared datasets.
- Develop interactive dashboards using Power BI.

## 👩‍💻 Author

**Anagha Sajeev**

 Data Analyst Intern | Python | Pandas | NumPy | Matplotlib | Seaborn | SQL | Power BI

---

⭐ This repository documents my learning journey in Exploratory Data Analysis and Python-based data preprocessing. Feedback and suggestions are welcome!
