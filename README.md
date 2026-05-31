# Customer Retail Data Analysis and Classification

## Project Overview

This project demonstrates a complete Machine Learning workflow for customer retail data classification. The main objective is to build, train, evaluate, and compare multiple Machine Learning models to predict customer classes (High Purchase Value vs. Low Purchase Value) based on retail transaction data.

The project covers data preprocessing, feature engineering, data visualization, model training, performance evaluation, and model comparison using different classification algorithms.

---

## Dataset Description

The customer retail dataset contains transaction-related information, including:

* InvoiceNo
* StockCode
* Description
* Quantity
* InvoiceDate
* UnitPrice
* CustomerID
* Country

### Features Used

The following features were selected for model training:

* Quantity
* UnitPrice
* Country

---

## Project Workflow

### 1. Library Imports and Setup

Necessary Python libraries are imported for:

* Data manipulation (`Pandas`, `NumPy`)
* Data visualization (`Matplotlib`)
* Data preprocessing (`LabelEncoder`)
* Model training and testing (`Scikit-learn`)
* Model evaluation (`Accuracy Score`, `Confusion Matrix`)

---

### 2. Data Loading and Initial Inspection

* Load the dataset into a Pandas DataFrame.
* Display the first few records.
* Check dataset structure and identify missing values.

---

### 3. Data Preprocessing

#### Handling Missing Values

Rows containing missing values are removed to ensure data quality and improve model performance.

#### Feature Selection

The following features are selected:

* Quantity
* UnitPrice
* Country

#### Encoding Categorical Data

Since machine learning algorithms require numerical input, the Country column is converted into numerical format using Label Encoding.

---

### 4. Feature Engineering and Target Variable Creation

#### Purchase Value Calculation

A new feature called **PurchaseValue** is created using:

PurchaseValue = Quantity × UnitPrice

#### Customer Class Creation

A target variable named **CustomerClass** is generated:

* 1 = High Purchase Value
* 0 = Low Purchase Value

The classification is based on the median PurchaseValue of the dataset.

---

### 5. Exploratory Data Analysis (EDA)

#### Customer Distribution by Country

A bar chart is created to visualize the top countries based on customer transactions. This helps understand customer distribution across different regions.

---

### 6. Model Training and Evaluation

#### Train-Test Split

The dataset is divided into:

* 80% Training Data
* 20% Testing Data

#### Machine Learning Models Implemented

##### Logistic Regression

A linear classification algorithm used for binary classification problems.

##### Decision Tree Classifier

A tree-based algorithm capable of learning complex patterns and decision rules.

##### K-Nearest Neighbors (KNN)

A distance-based classification algorithm that predicts classes using the nearest neighboring observations.

---

### 7. Model Evaluation

The performance of each model is measured using:

#### Accuracy Score

Measures the percentage of correctly classified records.

#### Confusion Matrix

Displays:

* True Positives
* True Negatives
* False Positives
* False Negatives

Confusion matrices are visualized to better understand model predictions.

---

### 8. Model Comparison

#### Accuracy Comparison Graph

A bar chart is generated to compare the accuracy scores of:

* Logistic Regression
* Decision Tree Classifier
* K-Nearest Neighbors (KNN)

This comparison helps identify the best-performing model for the dataset.

---

## Learning Outcomes

After completing this project, students will be able to:

* Understand the complete Machine Learning workflow.
* Perform data preprocessing and feature engineering.
* Handle missing values effectively.
* Encode categorical variables.
* Visualize data using graphs.
* Train multiple supervised learning models.
* Evaluate models using Accuracy Score and Confusion Matrix.
* Compare different Machine Learning algorithms.
* Interpret model results and visualizations.

---

## Conclusion

This project demonstrates how different Machine Learning algorithms perform on the same customer retail dataset. By applying data preprocessing, feature engineering, visualization, model training, and evaluation techniques, students gain practical experience in supervised learning.

The comparison of model accuracy scores and confusion matrices helps identify the most suitable algorithm for the given dataset.

### Summary of Models

* **Logistic Regression** performs well when the relationship between features and target classes is relatively linear.
* **Decision Tree Classifier** can capture complex patterns and is easy to interpret.
* **K-Nearest Neighbors (KNN)** classifies observations based on similarity and distance between data points.

Overall, the project provides a strong foundation for understanding Machine Learning model development, evaluation, and comparison in real-world retail data analysis.
