# Notebook publication guide
Add the existing notebooks under descriptive names. Suggested sequence:
1. `01_hotel_booking_eda.ipynb`: provenance, data checks, exploration and supported observations.
2. `02_regression.ipynb`: continuous target, preprocessing, baseline, linear regression and evaluation.
3. `03_classification.ipynb`: labels, class balance, baseline, logistic regression and evaluation.

These are suggested names, not existing files. Preserve the actual completed methodology; document any later corrections separately.

Before publishing, remove secrets, private paths and personal data. Check leakage and train/test separation, record seeds and dependencies, then restart the kernel and run all cells. Export readable figures to `reports/figures/` and link results to the relevant notebook.
