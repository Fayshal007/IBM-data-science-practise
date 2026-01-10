# Used Cars Pricing – Data Importing & Cleaning Project 🚗📊

![Python](https://img.shields.io/badge/Python-3.x-blue?logo=python)
![Pandas](https://img.shields.io/badge/Pandas-Data%20Analysis-purple?logo=pandas)
![NumPy](https://img.shields.io/badge/NumPy-Scientific%20Computing-blue)
![Jupyter Notebook](https://img.shields.io/badge/Jupyter-Notebook-orange?logo=jupyter)
![GitHub](https://img.shields.io/badge/GitHub-Repository-black?logo=github)
![License](https://img.shields.io/badge/License-MIT-yellow)

---

## 📌 Project Overview

This project focuses on **importing, cleaning, and preparing a real-world used cars pricing dataset** using **Python, Pandas, Numpy, Matplotlib** in a **Jupyter Notebook** environment.

The notebook demonstrates essential **data preprocessing techniques** that are critical before performing exploratory data analysis or machine learning.

---

## 👤 My Key Code Contribution

To prevent duplicate columns from being created when the notebook is executed multiple times, I implemented a conditional check before concatenating dummy variables.

### 🔹 Problem
Running the dummy-variable creation cell multiple times was adding **duplicate encoded columns**, which could corrupt the dataset and affect downstream analysis.

### 🔹 Solution (Implemented by Me)

```python
# My contribution to avoid adding duplicate dummy columns
if "fuel-type-diesel" not in df.columns:
    df = pd.concat([df, dummy_var], axis=1)
    df.drop("fuel-type", axis=1, inplace=True)
```

---

## 🛠️ Skills Demonstrated

### 🔹 Technical Skills
- Python programming
- Data importing and preprocessing
- Data cleaning & wrangling
- Handling missing values
- Data type conversion
- Data Standardization
- Data Normalization
- Binning
- Label categories to numerical variable

### 🔹 Libraries Used
- `pandas`
- `numpy`
- `matplotlib`

---

## 📊 Dataset Information

- Dataset: **Used Cars Pricing Dataset**
- Format: CSV
- Type: Real-world structured data
- Use case: Data preprocessing for analysis and machine learning

---

## 🎯 Learning Outcomes

Through this project, I gained hands-on experience in:

- Cleaning messy real-world datasets
- Applying data preprocessing techniques using Pandas
- Preparing data for exploratory data analysis and predictive modeling
- Following industry-standard data analysis workflows