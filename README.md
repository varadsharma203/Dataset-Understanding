# Dataset-Understanding
Exploratory Data Analysis (EDA) on the Titanic dataset to identify data types, missing values, and ML suitability using Pandas and NumPy.
# Task 1: Understanding Dataset & Data Types

 📌 Project Overview
The objective of this task is to load a dataset, analyze its structure, identify data types, and assess its readiness for Machine Learning models.

Selected Dataset: Titanic Dataset 

## 🛠️ Tools & Libraries Used
* **Language:** Python 
***Environment:** Google Colab / Jupyter Notebook 
***Libraries:** Pandas, NumPy, Seaborn (for data loading)

---

## 📊 Dataset Analysis Report*
### 1. Dataset Structure
* **Rows & Columns:** The dataset was loaded using Pandas. It contains **891 rows** and **15 columns**.
* **Target Variable:** `survived` (Binary: 0 = No, 1 = Yes).
* **Input Features:** Key features include `pclass` (Class), `sex`, `age`, `fare`, and `embarked`.

### 2. Data Types Identification
* **Numerical:** `age`, `fare`, `sibsp` (siblings/spouses), `parch` (parents/children).
* **Categorical:** `embarked`, `deck`, `who`, `embark_town`.
* **Ordinal:** `pclass` (1st > 2nd > 3rd), `class` (First, Second, Third).
* **Binary:** `sex` (male/female), `survived`, `adult_male`.

### 3. Statistical Summary & Data Quality 
* **Missing Values:**
    * The `deck` column has a significant number of missing values (>75%) and may need to be dropped.
    * The `age` column has roughly 20% missing values, which will require imputation (filling with mean/median).
* **Data Imbalance:**
    * The dataset shows an imbalance in the target variable `survived`.More passengers died (0) than survived (1), which is important to note for model training

### 4. Machine Learning Suitability
* **Readiness:** The dataset is **suitable** for introductory ML tasks (Classification).
* **Preprocessing Needed:**
    * Handling missing values in `age`.
    * Encoding categorical variables (converting `sex` and `embarked` to numbers).
    * Dropping irrelevant columns (e.g., `deck` due to nulls).

---

## 📂 Files in this Repository
* `Task_1_Titanic_Analysis.ipynb`: The Jupyter Notebook containing all Python code, data loading, and visualization steps.
* `README.md`: This file, serving as the documentation and analysis report.

## ⚙️ How to Run
1.  Clone this repository.
2.  Open `Task_1_Titanic_Analysis.ipynb` in Jupyter Notebook or Google Colab.
3.  Run all cells to view the outputs and analysis.
