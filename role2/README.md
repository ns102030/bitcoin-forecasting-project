# Role 2 – Model Training and Predictions

This folder contains all deliverables for **Role 2** of the Bitcoin Forecasting Project.  
Role 2 trains the forecasting models and produces the prediction outputs used by Role 3.

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
- Generate out-of-sample predictions for every model  
- Export the unified `predictions.csv` file used by Role 3  

---

## 📁 Folder Contents

- **`predictions.csv`**  
  The combined predictions file containing actual values, model forecasts, and the corresponding `Fold_ID`.

- **`notebooks/`**  
  Jupyter notebooks used for model training and prediction generation.

- **`scripts/`**  
  Python scripts containing reusable training and validation utilities.

---

## ▶️ How to Use

Load and inspect the predictions:

```python
import pandas as pd
df = pd.read_csv("predictions.csv")
df.head()
