# EDA Case Study — Loan Default Analysis

This is an exploratory data analysis (EDA) project on loan application data from a consumer finance company. The goal is to find patterns in the data that can help the company identify customers who are likely to default on their loan, so that they can make better lending decisions.

## Files

- `EDA_LoanDefault_Case_Study.ipynb` — the main Jupyter notebook with all the analysis
- `EDA_Presentation.html` — slide presentation of the key findings (open in a browser)

## How to Run

Make sure you have Python 3 with pandas, numpy, matplotlib, and seaborn installed:

```
pip install pandas numpy matplotlib seaborn
```

## Summary of Findings

Only 8.1% of applicants defaulted (TARGET=1), so the dataset is heavily skewed. All rates below are within-group percentages, not counts.

**What stood out:**

- **Income type** is the biggest differentiator. Unemployed applicants and those on maternity leave defaulted at 36–40%. Pensioners and state servants were down around 5–6%.
- **Age** shows a clean trend: default rates fall steadily as applicants get older. People in their 20s defaulted at 11.4%; people in their 60s at 4.9%.
- **Education** matters a lot too. Lower secondary holders defaulted at 10.9%, academic degree holders at just 1.8%.
- **Housing**: renters and people living with parents came in at 12.3%, noticeably higher than homeowners.
- **Past refusals** are a strong signal. Applicants who had 66–100% of their previous applications refused defaulted at 15%+, more than double the rate of those with no prior refusals.
- **Region**: applicants from the worst-rated areas (region 3) defaulted at 11.1% vs. 4.8% in the best-rated areas (region 1).
- **Credit-to-income ratio**: defaulters tended to borrow more relative to their income, which makes it a useful signal even when other variables look fine.

No single variable tells the full story, but together they give a much clearer picture of default risk!
