# Data Wrangling – Laptop Pricing Dataset

![Python](https://img.shields.io/badge/Python-3.x-blue?logo=python&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-Data%20Analysis-purple?logo=pandas&logoColor=white)
![NumPy](https://img.shields.io/badge/NumPy-Numerical%20Computing-lightblue?logo=numpy&logoColor=white)
![Matplotlib](https://img.shields.io/badge/Matplotlib-Visualization-orange)
![Jupyter Notebook](https://img.shields.io/badge/Jupyter-Notebook-orange?logo=jupyter&logoColor=white)

![Status](https://img.shields.io/badge/Status-Completed-brightgreen)
![License](https://img.shields.io/badge/License-Educational-lightgrey)
![Contributions](https://img.shields.io/badge/Contributions-Welcome-brightgreen)

![IBM Skills Network](https://img.shields.io/badge/IBM-Skills%20Network-blue?logo=ibm)
![Course](https://img.shields.io/badge/Course-Data%20Wrangling-success)

![Beginner Friendly](https://img.shields.io/badge/Level-Beginner-blue)
![Hands-On](https://img.shields.io/badge/Type-Hands--On-orange)



## 📌 Project Overview
This project is a **hands-on data wrangling practice lab** focused on cleaning, transforming, and preparing a laptop pricing dataset for analysis.  
The notebook demonstrates common real-world data preprocessing techniques using **Python, Pandas, NumPy, and Matplotlib**.

The goal is to transform raw, inconsistent data into a clean and structured format suitable for analysis or machine learning tasks.

---

## 📂 Dataset
- **Source:** IBM Skills Network / Coursera dataset  
- **File:** `laptop_pricing_dataset_mod1.csv`
- **Loaded directly from a URL** using Pandas

The dataset includes laptop specifications such as:
- Screen size
- Weight
- Price
- Other hardware-related attributes

---

## 🛠️ Tools & Libraries Used
- **Python 3**
- **NumPy** – numerical computations
- **Pandas** – data manipulation and cleaning
- **Matplotlib** – basic data visualization
- **Jupyter Notebook** – interactive execution

---

## 🔍 Tasks Performed

### 1️⃣ Import Required Libraries
Essential Python libraries are imported and configured for inline plotting.

---

### 2️⃣ Load the Dataset
The CSV file is loaded directly into a Pandas DataFrame using a remote URL.

---

### 3️⃣ Missing Data Evaluation
- Identifies missing (null) values in each column
- Uses `.isna()` and `.sum()` to quantify missing data

---

### 4️⃣ Handling Missing Values
- Numerical columns (e.g., `Weight_kg`) have missing values replaced with the **mean** of the column
- Ensures consistency and avoids dropping valuable records

---

### 5️⃣ Data Type Standardization
- Converts columns such as `Weight_kg` into proper numeric (`float`) data types
- Ensures accurate mathematical operations and analysis

---

### 6️⃣ Data Normalization
- Continuous variables are normalized to bring values onto a similar scale
- Helps improve comparability between features

---

### 7️⃣ Binning
- Continuous data is converted into categorical bins
- Useful for grouping values (e.g., low / medium / high ranges)

---

### 8️⃣ Categorical Variable Encoding
- Converts categorical variables into **dummy/indicator variables**
- Example:
  - The `Screen` column is transformed into binary columns such as:
    - `Screen Full HD`
- Original categorical column is dropped after encoding

---

## 📈 Output
- A cleaned and transformed Pandas DataFrame
- Ready for:
  - Exploratory Data Analysis (EDA)
  - Machine Learning models
  - Statistical analysis

---
