# Investigating Consumer Complaint Patterns and Response Trends in Financial Services

## Project Overview

This project investigates consumer complaint patterns and company response trends in the financial services sector using the Consumer Financial Protection Bureau (CFPB) Consumer Complaints dataset.

The objective is to identify frequently reported financial products and issues, examine changes in complaint volumes over time, analyse company response patterns and investigate differences in recorded date intervals.

Exploratory Data Analysis (EDA), data visualisation and statistical hypothesis testing were performed using Python.

## Business Objectives

- Identify financial products associated with the highest complaint volumes.
- Examine frequently reported consumer issues.
- Analyse annual and monthly complaint trends.
- Investigate changes in product-related complaint patterns over time.
- Examine company responses to consumer complaints.
- Analyse recorded date intervals between complaint submission and receipt.
- Apply statistical methods to identify associations and differences.
- Generate insights that may support improved customer service and complaint management.

## Dataset Description

**Source:** Consumer Financial Protection Bureau (CFPB) Consumer Complaints Database.

The dataset contains:

- **Total records:** 62,516
- **Original columns:** 12
- **Reporting period:** May 2017 – August 2023

Important variables include:

| Variable | Description |
|---|---|
| Complaint ID | Unique complaint identifier |
| Date submitted | Date the complaint was submitted |
| Date received | Date the complaint was received |
| Product | Financial product category |
| Sub-product | Specific financial product |
| Issue | Main complaint category |
| Sub-issue | Specific complaint issue |
| Company response to consumer | Recorded company response |
| Company public response | Public response information |
| Timely response? | Recorded timely response indicator |

## Tools and Technologies

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- SciPy
- Jupyter Notebook

## Data Preparation

The following data preparation activities were performed:

- Initial dataset inspection and structural analysis.
- Missing-value assessment.
- Duplicate-record checks.
- Examination of data types.
- Date-based feature engineering.
- Extraction of year and month from submission dates.
- Calculation of recorded date intervals between submission and receipt.
- Preparation of categorical data for statistical analysis.

Missing values were assessed according to their relevance rather than automatically removed.

## Research Questions

The project investigated four main research questions:

1. Does the distribution of complaints across financial product categories vary by year?
2. Is company response associated with financial product category?
3. Do positive recorded date intervals differ across financial product categories?
4. Is company response associated with the year of complaint submission?

## Exploratory Data Analysis

The exploratory analysis included:

- Annual complaint distribution.
- Monthly complaint distribution.
- Complaint distribution across financial products.
- Frequently reported complaint issues.
- Changes in product complaint patterns over time.
- Company response distribution.
- Company public response distribution.
- Recorded date interval analysis.

Visualisations were created using Matplotlib and Seaborn to communicate the findings.

## Statistical Analysis

The following statistical techniques were applied:

| Research question | Statistical technique |
|---|---|
| Product category and complaint year | Chi-square test of independence |
| Company response and product category | Chi-square test of independence |
| Positive recorded date intervals across products | Kruskal-Wallis test |
| Company response and complaint year | Chi-square test of independence |

A significance level of 0.05 was used.

Effect sizes were also calculated using Cramér's V for the Chi-square tests and epsilon-squared for the Kruskal-Wallis test.

## Key Findings

### 1. Financial Product Complaints

Checking and savings accounts recorded the highest number of complaints (24,814), followed by credit cards and prepaid cards (16,197).

Together, these categories accounted for approximately 65.6% of all complaints.

### 2. Frequently Reported Issues

Managing an account was the most frequently reported issue, with 15,109 complaints.

Other common issues included incorrect information on credit reports and problems with purchases appearing on statements.

### 3. Complaint Trends

Complaint volumes generally increased between 2017 and 2022, reaching a peak of 12,953 complaints in 2022.

The 2017 and 2023 reporting periods were incomplete.

### 4. Company Response Patterns

Approximately 65.65% of complaints were recorded as closed with an explanation.

Monetary and non-monetary relief together accounted for approximately 31.94%.

### 5. Recorded Date Intervals

Approximately 79.40% of complaints had the same submission and receipt calendar date.

Among complaints with positive recorded intervals, the median difference was 2 days.

### 6. Statistical Findings

- Product category and complaint year showed a statistically significant but very weak association (Cramér's V = 0.0881).
- Company response and product category showed a statistically significant but weak association (Cramér's V = 0.1723). This result requires caution because some expected cell frequencies were too small.
- Positive recorded date intervals differed significantly across product categories, with a small effect size (epsilon-squared = 0.0324).
- Company response and complaint year showed a statistically significant but weak association (Cramér's V = 0.2220).

All statistically significant results were reported at p < 0.001.

## Repository Structure

```text
Consumer_Complaints_Project/
│
├── Consumer_Complaints_Analysis.ipynb
│
├── Analytical_Report.docx
│
├── Consumer_Complaints.xlsx
│
├── Data_Dictionary.csv
│
├── VISUALIZATIONS/
│   ├── annual_complaints.png
│   ├── monthly_complaints.png
│   ├── product_distribution.png
│   └── other_visualizations.png
│
└── README.md
```

*The filenames shown for visualisations are illustrative. Replace them with your actual filenames.*

## How to Run the Project

1. Clone or download this repository.
2. Install the required Python libraries:

```bash
pip install pandas numpy matplotlib seaborn scipy openpyxl jupyter
```

3. Open Jupyter Notebook:

```bash
jupyter notebook
```

4. Open `Consumer_Complaints_Analysis.ipynb`.
5. Ensure the dataset is available at the file path specified in the notebook.
6. Run the notebook cells sequentially to reproduce the analysis.

## Limitations

- The dataset contains missing values in some categorical variables.
- The reporting periods for 2017 and 2023 are incomplete.
- CFPB complaints do not represent all dissatisfied financial-services consumers.
- Different financial products have different customer populations and transaction volumes.
- Recorded date intervals do not necessarily represent actual complaint-processing or resolution times.
- Some product categories have small sample sizes.
- The product-response Chi-square analysis did not fully satisfy expected-frequency assumptions.
- Statistical associations do not establish causation.

## Conclusion

This project demonstrates how consumer complaint data can be analysed to identify recurring service concerns, examine complaint trends and investigate company response patterns in the financial services sector.

The findings highlight the importance of account management, credit card services, transparent customer communication and regular monitoring of consumer complaints.

The project also demonstrates the application of exploratory data analysis, statistical hypothesis testing and data visualisation to a real-world business problem.

## Author

**Nikhila K. S.**

Data Science | Machine Learning | AI Enthusiast

