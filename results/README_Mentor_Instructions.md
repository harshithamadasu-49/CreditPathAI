# CreditPathAI —  (Milestones 2–4)

This folder contains:
- `credit_risk_dataset.csv` and `Loan_Default.csv` (original datasets)
- `train_all.py` — end-to-end: EDA, preprocessing, baseline model, advanced models, metrics, plots, PPTX and ZIP of results.
- `creditpath_results/` — created after running `train_all.py` and contains:
  - model pickles (*.pkl)
  - plots (*.png)
  - metrics_*.csv
  - CreditPathAI_report.pptx (if python-pptx available)
  - CreditPathAI_complete.zip

## How to run
1. Put `credit_risk_dataset.csv` and `Loan_Default.csv` in the same folder as `train_all.py`.
2. Install dependencies:
   pip install -r requirements.txt
   or at minimum:
pip install scikit-learn pandas numpy matplotlib python-pptx xgboost lightgbm
(xgboost/lightgbm optional — script will fallback to HistGradientBoosting if not present)
3. Run:
python train_all.py
4. After run, share `CreditPathAI_complete.zip` and `creditpath_results/CreditPathAI_report.pptx` with mentor.

## Checklist for mentor
- [ ] EDA graphs (target distribution, numeric distributions, correlation matrix)
- [ ] Preprocessing explained (missing values imputed, categorical encoded)
- [ ] Baseline model (Logistic Regression) + AUC and confusion matrix
- [ ] Advanced models (XGBoost / LightGBM or fallback) + comparison table
- [ ] Models saved as .pkl
- [ ] PPTX summary with results and next steps




