[README.md](https://github.com/user-attachments/files/27115719/README.md)
# ACC102-Track2-Credit-Card-Spending-Analysis# Credit Card Customer Spending Analysis

## Project Overview

This Track 2 GitHub data analysis project studies how customer income, age, and home ownership relate to average monthly credit card spending. The intended user is a junior credit card product analyst who wants a simple customer segmentation view before designing spending-related marketing or risk-monitoring actions.

## Analytical Question

Which customer characteristics are most strongly associated with higher average monthly credit card spending?

## Dataset

- Dataset name: William Greene credit card data
- Source: `statsmodels.datasets.ccard`, based on William Greene's *Econometric Analysis*
- Local file: `data/credit_card_spending.csv`
- Access date: 27 April 2026
- Observations: 72 customers
- Main variables:
  - `AVGEXP`: average monthly credit card expenditure
  - `AGE`: customer age
  - `INCOME`: customer income, measured in thousands
  - `OWNRENT`: home ownership indicator, where 1 means owner and 0 means renter

## Method

The Python workflow:

1. Loads the credit card spending dataset.
2. Renames variables into readable labels.
3. Creates income bands and a spend-to-income ratio.
4. Produces descriptive statistics and group summaries.
5. Creates visualisations for income band, income-spending relationship, and home ownership.
6. Fits a simple OLS regression model to estimate the relationship between spending and income, age, and home ownership.

## Main Findings

- Average monthly spending rises across income groups. High-income customers spend the most on average.
- The high-income group also has the highest average spend-to-income ratio in this sample.
- The regression result suggests that income is the strongest predictor in this dataset. The estimated coefficient for income is positive and statistically meaningful.
- Age and home ownership do not show strong explanatory power once income is included.

## Repository Structure

```text
.
├── data/
│   └── credit_card_spending.csv
├── notebooks/
│   └── credit_card_spending_analysis.ipynb
├── outputs/
│   ├── figures/
│   ├── home_ownership_summary.csv
│   ├── income_band_summary.csv
│   ├── model_summary.txt
│   ├── regression_results.csv
│   └── summary_statistics.csv
├── scripts/
│   └── analyze_credit_card_spending.py
├── submission_files/
│   ├── demo_video_script.md
│   └── reflection_report.md
├── README.md
└── requirements.txt
```

## How to Run

Install the required packages:

```bash
pip install -r requirements.txt
```

Run the analysis script:

```bash
python scripts/analyze_credit_card_spending.py
```

Or open and run the notebook:

```text
notebooks/credit_card_spending_analysis.ipynb
```

## Submission Notes

For ACC102 Track 2, submit:

- GitHub repository link
- Python notebook: `notebooks/credit_card_spending_analysis.ipynb`
- README file: `README.md`
- Demo video link, 1-3 minutes
- Reflection report: `submission_files/reflection_report.md`

