# 4_data_analysis

This folder contains the initial modeling step to predict whether renewables are more cost-efficient for a project.

## Objective

Build a classifier to estimate cost-efficiency of renewables using available project descriptors and cost fields.

## Approach

- Merge a system cost column (AED) into the main dataset by country if not already present.
- Simulate a target label by comparing a diesel baseline proxy with the system cost (AED).
- Train baseline models (Logistic Regression and Random Forest) and evaluate on a hold-out set.

## Outputs

- `modeling_notebook.ipynb` — end-to-end modeling workflow.
- `plots/confusion_matrix.png` — confusion matrix for the RandomForest model.
- `plots/feature_importance.png` — top features ranked by importance.
- `metrics.txt` — model accuracy, precision, and recall on the test split.
- `labeling_preview.csv` — sample of system cost, diesel cost proxy, and simulated label.

## How to Run Locally

1. Navigate to the repository root in your terminal.  
2. Install required packages if not already installed:

   ```bash
   pip install pandas scikit-learn matplotlib seaborn
   ```

3. Open the notebook:

   ```bash
   jupyter notebook 4_data_analysis/modeling_notebook.ipynb
   ```

4. Run all cells to reproduce the metrics and plots.  
   The outputs will be saved automatically in the `plots/` folder and `metrics.txt` file.
