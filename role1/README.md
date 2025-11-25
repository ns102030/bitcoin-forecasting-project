# Role 1 – Data Collection, Cleaning, and Feature Engineering

This folder contains all deliverables produced as part of **Role 1** of the Bitcoin Forecasting Project.  
Role 1 is responsible for preparing clean, structured, and feature-rich data for downstream modeling tasks.

---

## 📌 Responsibilities

- Collect historical Bitcoin price data from the chosen data source(s)
- Clean raw data (handle missing values, inconsistencies, formatting issues)
- Perform data preprocessing:
  - Sorting by timestamp
  - Filtering valid rows
  - Converting datatypes
  - Normalizing or scaling features (if required)
- Engineer features for predictive modeling
- Split or prepare the dataset for model training
- Export the cleaned dataset to be used by Role 2

---

## 📁 Files in This Folder

- `dataset_clean.csv`  
  The final cleaned dataset used by Role 2 for model training and cross-validation.

- `notebooks/`  
  Jupyter notebooks used during data collection, exploration, and feature engineering.

- `scripts/`  
  Optional Python scripts for reusable data preprocessing logic.

---

## ▶️ How to Use

To load the cleaned dataset in Python:

```python
import pandas as pd

df = pd.read_csv("dataset_clean.csv")
print(df.head())
