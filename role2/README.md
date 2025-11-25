
---

# 🟩 **role2/README.md**  
### *Model Training and Predictions*

```markdown
# Role 2 – Model Training and Predictions

This folder contains all deliverables produced as part of **Role 2** of the Bitcoin Forecasting Project.  
Role 2 is responsible for training machine learning and time-series models and generating out-of-sample predictions.

---

## 📌 Responsibilities

- Load the cleaned dataset from Role 1
- Train multiple forecasting models, including:
  - K-Nearest Neighbors (KNN)
  - XGBoost
  - LightGBM
  - ARIMA
  - LSTM
- Perform **TimeSeriesSplit** cross-validation to ensure chronological integrity
- Generate predictions for each model across all validation folds
- Export a unified predictions file for Role 3

---

## 📁 Files in This Folder

- `predictions.csv`  
  Contains actual values, predicted values for each model, and the corresponding `Fold_ID`.

- `notebooks/`  
  Jupyter notebooks used to train models and generate predictions.

- `scripts/`  
  Optional Python files containing reusable model-training utilities.

---

## ▶️ predictions.csv Format

Columns typically include:

- `Date` – Timestamp for each prediction  
- `Actual_Price` – Ground-truth Bitcoin closing price  
- `Pred_KNN`, `Pred_XGB`, `Pred_LGBM`, etc. – Model predictions  
- `Fold_ID` – Identifies which cross-validation fold each prediction belongs to  

This file is directly consumed by Role 3.

---

## ▶️ Running the Role 2 Notebook

Activate your environment and run:

```bash
jupyter notebook
