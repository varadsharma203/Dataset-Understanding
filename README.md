# Dataset-Understanding
Exploratory Data Analysis (EDA) on the Titanic dataset to identify data types, missing values, and ML suitability using Pandas and NumPy.
# Task 1: Understanding Dataset & Data Types

### 🚀 Elevate Labs AI & ML Internship
**Submission by:** [Your Name]  
**Date:** February 11, 2026

---

## 📌 Project Overview
[cite_start]This repository contains the submission for **Task 1** of the AI & ML Internship[cite: 3]. [cite_start]The objective of this task is to load a dataset, analyze its structure, identify data types, and assess its readiness for Machine Learning models[cite: 25].

[cite_start]**Selected Dataset:** Titanic Dataset [cite: 11]

## 🛠️ Tools & Libraries Used
* [cite_start]**Language:** Python [cite: 5]
* [cite_start]**Environment:** Google Colab / Jupyter Notebook [cite: 6]
* [cite_start]**Libraries:** Pandas, NumPy, Seaborn (for data loading) [cite: 5]

---

## 📊 Dataset Analysis Report
[cite_start]*(Deliverable: 1-Page Analysis)* [cite: 23]

### 1. Dataset Structure
* **Rows & Columns:** The dataset was loaded using Pandas. It contains **891 rows** and **15 columns**.
* [cite_start]**Target Variable:** `survived` (Binary: 0 = No, 1 = Yes)[cite: 18].
* **Input Features:** Key features include `pclass` (Class), `sex`, `age`, `fare`, and `embarked`.

### [cite_start]2. Data Types Identification [cite: 15]
* **Numerical:** `age`, `fare`, `sibsp` (siblings/spouses), `parch` (parents/children).
* **Categorical:** `embarked`, `deck`, `who`, `embark_town`.
* **Ordinal:** `pclass` (1st > 2nd > 3rd), `class` (First, Second, Third).
* **Binary:** `sex` (male/female), `survived`, `adult_male`.

### [cite_start]3. Statistical Summary & Data Quality [cite: 16, 20]
* **Missing Values:**
    * The `deck` column has a significant number of missing values (>75%) and may need to be dropped.
    * The `age` column has roughly 20% missing values, which will require imputation (filling with mean/median).
* **Data Imbalance:**
    * The dataset shows an imbalance in the target variable `survived`. [cite_start]More passengers died (0) than survived (1), which is important to note for model training[cite: 30].

### [cite_start]4. Machine Learning Suitability [cite: 19]
* **Readiness:** The dataset is **suitable** for introductory ML tasks (Classification).
* **Preprocessing Needed:**
    * Handling missing values in `age`.
    * Encoding categorical variables (converting `sex` and `embarked` to numbers).
    * Dropping irrelevant columns (e.g., `deck` due to nulls).

---

## 📂 Files in this Repository
* [cite_start]`Task_1_Titanic_Analysis.ipynb`: The Jupyter Notebook containing all Python code, data loading, and visualization steps[cite: 22].
* [cite_start]`README.md`: This file, serving as the documentation and analysis report[cite: 43].

## ⚙️ How to Run
1.  Clone this repository.
2.  Open `Task_1_Titanic_Analysis.ipynb` in Jupyter Notebook or Google Colab.
3.  Run all cells to view the outputs and analysis.
