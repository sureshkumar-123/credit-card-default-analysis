# Credit Card Default Analysis & Visualization using Python

Exploratory data analysis (EDA) of credit card customers to understand which characteristics and repayment behaviours are linked to payment default.

**Tech stack:** Python, NumPy, Pandas, Matplotlib, Seaborn

## Dataset
[Default of Credit Card Clients](https://archive.ics.uci.edu/dataset/350/default+of+credit+card+clients) (UCI Machine Learning Repository, also available on Kaggle): 30,000 customers with demographics, credit limit, 6 months of repayment status, bill amounts and payment amounts, plus a target column showing default in the next month.

## What the analysis covers
1. Data loading and inspection
2. Data cleaning: missing values, duplicate rows, undocumented category codes (`EDUCATION`, `MARRIAGE`)
3. Overall default rate
4. Default rate by gender, education and marital status
5. Credit limit and age group analysis
6. Repayment history (`PAY_1` to `PAY_6`) and number of delayed months
7. Credit utilization and bill vs payment trends
8. Correlation heatmap
9. Key insights generated directly from the data

## Project structure
```
credit-card-default-analysis/
├── credit_card_default_analysis.ipynb   # main analysis notebook
├── data/                                # place the dataset here (not committed)
├── images/                              # charts saved by the notebook
├── requirements.txt
└── README.md
```

## How to run
```bash
git clone https://github.com/<your-username>/credit-card-default-analysis.git
cd credit-card-default-analysis
pip install -r requirements.txt
```
1. Download the dataset from UCI or Kaggle and save it as `data/UCI_Credit_Card.csv`.
2. Start Jupyter and run all cells:
```bash
jupyter notebook credit_card_default_analysis.ipynb
```

## Results
Charts are saved in the `images/` folder and the notebook prints a summary of key insights at the end.

## Possible next steps
- Build a predictive model (logistic regression, random forest) using these features
- Build a Tableau dashboard from the cleaned data
