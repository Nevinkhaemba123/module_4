# Breast Cancer Classification & Exploratory Data Analysis (EDA)

## Project Overview
This repository contains a complete exploratory data analysis (EDA) and machine learning preprocessing workflow using the **Breast Cancer Wisconsin Dataset**. The project demonstrates data loading, persistence, data cleaning, class distribution analysis, and target label standardization using Python data science libraries (`pandas`, `numpy`, `matplotlib`, `seaborn`, and `scikit-learn`).

---

## Dataset Information
* **Source**: `scikit-learn` built-in datasets (`load_breast_cancer`).
* **Dimensions**: 569 samples, 30 numerical feature columns, and 1 target column.
* **Features**: Computed characteristics from digitized images of fine needle aspirate (FNA) breast masses (e.g., radius, texture, perimeter, area, smoothness, compactness, concavity, symmetry, and fractal dimension).
* **Target Variable**: 
  * *Original Labeling*: `0` = malignant, `1` = benign.
  * *Mapped Labeling*: Standardized to `1` = malignant, `0` = benign for modeling clarity.

---

## Notebook Structure & Workflow

1. **Environment Setup & Imports**: Imports core libraries for data manipulation, visualization, and modeling (`pandas`, `numpy`, `matplotlib`, `seaborn`, `scikit-learn`).
2. **Data Acquisition & Persistence**: Extracts the dataset as a pandas DataFrame and exports it locally as `breast_cancer.csv`.
3. **Data Inspection & Quality Checks**: 
   * Verifies dataset dimensions `(569, 31)`.
   * Checks data types, non-null counts, and missing values (`df.info()`).
   * Generates statistical summaries (`df.describe()`).
4. **Exploratory Data Analysis (EDA)**:
   * Examines target class counts and percentage distributions.
   * Remaps and standardizes target classes.
   * Visualizes feature distributions and relationships using Seaborn.

---

## Getting Started

### Prerequisites
Ensure you have Python installed along with the required libraries:
```bash
pip install pandas numpy matplotlib seaborn scikit-learn
