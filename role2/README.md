Role 2 – Model Training and Predictions

This folder contains all deliverables for Role 2 of the Bitcoin Forecasting Project.
Role 2 is responsible for training machine learning and time-series models and generating predictions for evaluation in Role 3.

📌 Responsibilities

Load the cleaned dataset produced by Role 1

Train multiple forecasting models, including:

K-Nearest Neighbors (KNN)

XGBoost

LightGBM

ARIMA

LSTM

Use TimeSeriesSplit cross-validation to maintain chronological integrity

Generate out-of-sample predictions for each fold

Export all predictions into a single predictions.csv file

Ensure consistent column names and alignment with actual prices

📁 Folder Contents

predictions.csv
Unified predictions file used by Role 3. Contains actual values, model predictions, and Fold_ID.

notebooks/
Jupyter notebooks used to train models and generate predictions.

scripts/
Python files containing model training utilities, preprocessing helpers, and cross-validation logic.

▶️ predictions.csv Format

Typical columns include:

Date — Timestamp for each prediction

Actual_Price — True Bitcoin close price

Pred_KNN — KNN model prediction

Pred_XGB — XGBoost model prediction

Pred_LGBM — LightGBM model prediction

Pred_ARIMA — ARIMA model prediction

Pred_LSTM — LSTM neural network prediction

Fold_ID — Cross-validation fold identifier

This file is the sole required input for Role 3.

▶️ Running the Role 2 Notebook

Activate your virtual environment (optional):

python -m venv .venv
.\.venv\Scripts\activate


Install dependencies:

pip install -r ../requirements.txt


Start Jupyter Notebook:

jupyter notebook


Open the notebook in notebooks/, run all cells to retrain models and regenerate predictions.csv.

🔗 Output Provided to Role 3

Role 2 provides the following final deliverable:

predictions.csv — containing predictions from every trained model, used directly by Role 3 for metric computation and visualization.

📝 Notes

Ensure the dataset from Role 1 is properly loaded and preprocessed before training models.

Double-check that all predictions align correctly with actual timestamps.

Model performance in Role 3 relies entirely on the correctness of the predictions generated here.
