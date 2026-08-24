# Week 3 — Statistical Analysis and Hypothesis Testing

## Project Overview
This project focuses on applying statistical analysis and hypothesis testing
to the Superstore dataset using Python. The main objective is to determine
whether observed differences in profitability are statistically significant
and to understand what these findings may mean from a business perspective.

## Objectives
- Analyze the relationship between discount levels and profit.
- Test whether average profit differs between low- and high-discount groups.
- Measure the difference using a 95% confidence interval and Cohen's d.
- Test whether average profit differs across product categories.
- Use Tukey HSD to identify which category pairs differ significantly.
- Present the results using clear visualizations.

## Dataset
The project uses the Superstore sales dataset containing 9,994 records.
The analysis mainly uses the Sales, Quantity, Discount, Profit, and Category
variables.

## Statistical Methods
The following methods were used:
- Welch's independent-samples t-test
- 95% confidence interval
- Cohen's d effect size
- One-way ANOVA
- Tukey HSD post-hoc test

## Key Findings

### Discount and Profit
Orders with discounts below 30% had an average profit of approximately
$49.04, while orders with discounts of 30% or more had an average profit
of approximately -$97.18.

The Welch's t-test produced:
- t-statistic: 16.141
- p-value: 2.295 × 10⁻⁵⁴
- Mean difference: $146.22
- 95% confidence interval: $128.45 to $163.99
- Cohen's d: 0.6393

The results show a statistically significant difference in average profit
between the two discount groups.

### Product Category and Profit

Average profit by category:
- Technology: $78.75
- Office Supplies: $20.33
- Furniture: $8.70

One-way ANOVA produced:
- F-statistic: 54.311
- p-value: 3.470 × 10⁻²⁴

Tukey HSD showed that Technology had significantly higher average profit
than both Furniture and Office Supplies, while the difference between
Furniture and Office Supplies was not statistically significant.

## Visualizations
The repository contains visualizations supporting the statistical analysis,
including comparisons of profit by discount group and product category.

## Project Structure
Week3-Statistical-Analysis/
│
├── Week3_Statistical_Analysis.ipynb
├── Week3_Statistical_Analysis_Report.docx
│
├── data/
│   └── Superstore.csv
│
└── visualizations/
    ├── profit_by_discount_group.png
    └── profit_by_category.png

## Tools and Libraries
- Python
- Pandas
- NumPy
- SciPy
- Statsmodels
- Matplotlib
- Seaborn
- Jupyter Notebook

## Conclusion
The analysis provides strong statistical evidence that profit differs across
discount groups and product categories. The results demonstrate how
hypothesis testing can be used to support data-driven business decisions.

## Author
Avani Chauhan