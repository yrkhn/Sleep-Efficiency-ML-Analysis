# Sleep Efficiency - ML Analysis

Two machine learning notebooks built on the **Sleep Efficiency Dataset** (452 records, 2021). The dataset contains physiological and lifestyle features for predicting how efficiently a person sleeps.

---

## Notebooks

### `assignment_1_sleep_efficiency_final.ipynb` — Regression
Predicts sleep efficiency as a continuous value (0–1).

- Preprocessing: cyclic encoding of bedtime/wakeup, median imputation, label encoding
- EDA: distribution plots, correlation heatmap, feature scatter plots
- Models: **Linear Regression** vs **Random Forest Regressor**
- Best result: Random Forest — **R² = 0.884**, RMSE = 0.049

### `midterm.ipynb` — Classification
Predicts sleep efficiency class: **Low** (< 0.70) vs **High** (≥ 0.70).

- Models: **Logistic Regression**, **KNN** (k tuned via cross-validation), **Decision Tree**
- Best result: Decision Tree — **Accuracy = 86.8%**, F1 = 0.857

---

## Key Findings

- Deep sleep percentage and number of awakenings are the strongest predictors of sleep quality
- Smoking and alcohol consumption have a notable negative effect
- Random Forest and Decision Tree outperform linear models on this dataset

---

## Stack

- Python 3
- `pandas`, `numpy`, `matplotlib`, `seaborn`
- `scikit-learn`

---

## How to Run

```bash
pip install pandas numpy matplotlib seaborn scikit-learn jupyter
jupyter notebook
```

Open either notebook and place `Sleep_Efficiency.csv` in the same folder.
