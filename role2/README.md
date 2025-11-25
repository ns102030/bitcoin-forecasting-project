---

  
Role 2

```markdown
# Role 2 – Model Training and Predictions

This folder contains all deliverables for **Role 2** of the Bitcoin Forecasting Project.  
Role 2 trains forecasting models and produces prediction outputs for Role 3.

---

## 📌 Responsibilities

- Load the cleaned dataset provided by Role 1  
- Train multiple forecasting models:  
  - KNN  
  - XGBoost  
  - LightGBM  
  - ARIMA  
  - LSTM  
- Use **TimeSeriesSplit** for chronological cross-validation  
- Generate out-of-sample predictions for every fold  
- Export all predictions in a unified `predictions.csv` file  

---

## 📁 Folder Contents

- **`predictions.csv`**  
  Contains actual values, model predictions, and the `Fold_ID` used by Role 3.

- **`notebooks/`**  
  Jupyter notebooks for model training and prediction generation.

- **`scripts/`**  
  Python utilities for reusable modeling logic.

---

## ▶️ `predictions.csv` Format

Common columns:

- `Date`  
- `Actual_Price`  
- `Pred_KNN`  
- `Pred_XGB`  
- `Pred_LGBM`  
- `Pred_ARIMA`  
- `Pred_LSTM`  
- `Fold_ID`  

---

## ▶️ Running the Role 2 Notebook

1. Create/activate virtual environment (optional):

```bash
python -m venv .venv
.\.venv\Scripts\activate here.
