# Customer Churn Prediction MLFLOW -Lab

## Overview
This lab predicts telecom customer churn using machine learning with MLflow for experiment tracking, model registration, and deployment.

## Dataset
**IBM Telco Customer Churn** — [Kaggle Link](https://www.kaggle.com/datasets/blastchar/telco-customer-churn)
- 7,043 customers with 21 features
- Target: `Churn` (Yes/No → binary)
- Features include tenure, contract type, monthly charges, internet service, payment method, etc.

## Project Structure
```
MLflow-Lab-2/
├── data/
│   └── Telco-Customer-Churn.csv
├── mlruns/
├── starter.ipynb
├── requirements.txt
└── README.md
```

## Modifications from Original Lab
1. **Different dataset** — Telco Customer Churn instead of Wine Quality
2. **Categorical encoding** — Added Label Encoding for 9 categorical features
3. **Correlation heatmap** — Additional EDA visualization
4. **Second model (XGBoost)** — Compared against Random Forest baseline
5. **Dynamic model registration** — Best model selected automatically

## Results

### Model Comparison
| Model | AUC Score |
|-------|-----------|
| Random Forest | 
0.78 |
| XGBoost |0.84 |

### MLflow Experiment Tracking and MLflow Model Details

<img width="956" height="437" alt="Image" src="https://github.com/user-attachments/assets/e3fb7033-ab44-4431-b1e4-dd5242e16b2c" />

<img width="1909" height="890" alt="Image" src="https://github.com/user-attachments/assets/b32181d7-46ae-49a3-8309-d70c9f99a8ff" />

<img width="1919" height="957" alt="Image" src="https://github.com/user-attachments/assets/51525413-939e-41e8-9cff-bdf66be2c2c2" />


## How to Run
1. Clone the repo: `git clone https://github.com/VaraalakshimeV/MLflow-Lab-2.git`
2. Install dependencies: `pip install -r requirements.txt`
3. Download dataset from [Kaggle](https://www.kaggle.com/datasets/blastchar/telco-customer-churn) and place in `data/` folder
4. Run `starter.ipynb` step by step
5. View MLflow UI: `python -m mlflow ui` then open `http://localhost:5000`

## Tools & Libraries
- scikit-learn, XGBoost — Model training
- MLflow — Experiment tracking, model registry, deployment
- Pandas, NumPy — Data processing
- Seaborn, Matplotlib — Visualization

## Author
Varaalakshime V — Northeastern University, MS Data Analytics Engineering
