# taplend-loan-case-study

TapLend Loan Approval Case Study

Analysis of 634 approved loans to decide which new applicants TapLend should approve.

Files
analysis.ipynb: the full analysis
chart_bad_rate.png: bad rate by pay frequency, FICO score and age

The data file (AssessmentDataScientist.xlsx) is not included because it is company data with personal details.

How to run
Put AssessmentDataScientist.xlsx next to the notebook.
Install the libraries: pip install pandas openpyxl scikit-learn matplotlib seaborn
Run the notebook cells from top to bottom.
Main findings
55% of the matched loans went bad.
Pay frequency, FICO retail score, age and direct deposit carried the most signal.
Logistic regression reached AUC 0.665 in cross-validation, but 0.588 on a time-based test, so I treat it as a pilot-stage model.
Everyone in the data was already approved, so declined applicants are missing (selection bias).
