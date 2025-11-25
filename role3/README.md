# Role 3 – Evaluation, Metrics, and Visualization

This folder contains all deliverables for **Role 3** of the Bitcoin Forecasting Project.  
Role 3 evaluates model performance and produces the final metrics and visualizations.

---

## 📌 Responsibilities

- Load `predictions.csv` from Role 2  
- Compute evaluation metrics:  
  - RMSE  
  - MAE  
  - MAPE  
  - R²  
  - Directional Accuracy (DA)  
- Create model comparison tables  
- Generate plots, including:  
  - Actual vs Predicted  
  - RMSE  
  - MAE  
  - MAPE  
  - R²  
  - DA  
- Export all metrics and figures for inclusion in the final report and presentation  

---

## 📁 Folder Contents

- **`role3_evaluation_notebook.ipynb`**  
  Notebook that computes metrics and generates visualizations.

- **`metrics_summary.csv`**  
  Final combined metrics table for all models.

- **`plots/`**  
  Folder containing exported charts produced by the notebook.

---

## ▶️ How to Use

Run the evaluation notebook with:

```bash
jupyter notebook role3_evaluation_notebook.ipynb
