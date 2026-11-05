# 2025 NYC Business Improvement District Analysis

*Exploratory Data Analysis | Python | Pandas | Data Visualization | Business Analytics*

---

## Project Overview

This project presents an exploratory data analysis of New York City's 2025 Business Improvement District (BID) data, covering **76 BIDs across the five boroughs**.

The objective is to examine reported financial, operational, staffing, sanitation, public-safety, and marketing indicators to identify patterns, compare resource allocation, and explore relationships between selected variables.

Using Python and statistical analysis, the project investigates how BID activities and reported resources vary across districts and boroughs, translating publicly reported information into meaningful business insights.

## Key Findings

### 1. Geographic and Economic Concentration

The analysis covers **76 BIDs**: Manhattan has the largest number of districts (26), followed by Brooklyn (23), the Bronx (12), Queens (11), and Staten Island (4). Manhattan also accounts for the largest reported aggregate revenue, expenses, and business counts across the five boroughs.

### 2. Reported Business Activity

BIDs report a combined **69,454 individual businesses** across their service areas, including 49,261 in Manhattan. These figures represent BID-reported business counts and should not be interpreted as unique citywide storefront estimates.

### 3. Resource Allocation

Manhattan has the highest median total spending, sanitation spending, and streetscape spending per linear foot. Staten Island has the lowest median total and sanitation spending intensity, while the Bronx has the lowest median streetscape spending intensity.

### 4. Sanitation and Service Activity

The rankings identify substantial differences in reported sanitation activity, staffing, and spending across individual BIDs. These measures describe reported activity and resource allocation rather than service quality or operational efficiency.

### 5. Public Safety

Manhattan has the highest median reported public-safety interactions per program hour among boroughs with usable observations.

Results should be interpreted cautiously because reporting coverage varies considerably, including only two valid observations for Queens and none for Staten Island.

### 6. Marketing and Community Engagement

Marketing materials distributed show virtually no linear association with estimated event attendance on the original scale (Pearson r = -0.009), although the rank-based relationship is moderately positive (Spearman ρ = 0.561).

Digital subscribers and estimated event attendance show a strong original-scale Pearson correlation (r = 0.917). However, this relationship is sensitive to extreme observations, particularly Times Square Alliance.

Excluding Times Square reduces the original-scale correlation to 0.162, while the log-scale relationship remains positive at 0.581. This highlights the importance of examining outliers and measurement scale when interpreting correlations.

### 7. Staffing Density

Manhattan has the highest median total staff and sanitation workers per service-area mile. Staten Island has the lowest median total staff per mile, followed by the Bronx.

Staffing comparisons reflect reported headcount rather than full-time-equivalent staffing, and the categories may overlap.

### 8. Sanitation Service Models

BIDs reporting in-house sanitation services have higher median sanitation spending per linear foot and more sanitation workers per mile than contracted BIDs.

These differences may reflect district size, resources, and service requirements rather than differences in operational efficiency.

### 9. Assessment Dependence

Assessment revenue represents a substantial funding source across BIDs, with an overall median dependence of **80.85%**.

The largest-expenditure quartile has higher median assessment dependence than the smallest-expenditure quartile, although this exploratory comparison does not establish causation.

### 10. Administrative Spending

The G&A analysis includes **49 of the 76 BIDs (64.5%)** with complete reporting across all six expense categories.

The remaining 27 BIDs have at least one unreported category. Results are therefore indicative of the reporting subset rather than the full BID network, and Staten Island is not represented in the G&A scatterplot.

---

## Methodology

The analysis includes:

- Data cleaning, type conversion, and missing-value assessment.
- Exploratory data analysis and descriptive statistics.
- Borough-level comparisons using medians and distributions.
- Normalized spending and staffing measures per linear foot or service-area mile.
- Sanitation and public-safety activity ratios.
- Marketing correlations using Pearson and Spearman methods.
- Logarithmic transformations and sensitivity analysis excluding Times Square Alliance.
- Assessment revenue dependence and G&A expense calculations.
- Data visualization using Matplotlib and Seaborn.

## Tools & Technologies

- **Python** — Data analysis and programming.
- **Pandas** — Data manipulation and cleaning.
- **NumPy** — Numerical computations.
- **Matplotlib** — Data visualization.
- **Seaborn** — Statistical visualization.
- **adjustText** — Improving chart annotations.
- **Jupyter Notebook** — Interactive analysis and documentation.

## Project Structure

```text
2025-nyc-bid-analysis/
│
├── README.md
├── .gitignore
│
├── notebooks/
│   └── Jupyter notebooks
│
├── reports/
│   └── Exported HTML reports
│
└── figures/
    └── PNG visualizations
```

## Limitations & Considerations

1. The analysis relies on reported BID data, and reporting coverage varies across variables and boroughs.
2. Missing values are not automatically treated as zero. Complete-case requirements reduce the number of observations for certain analyses.
3. BID-reported business counts may not represent unique storefronts citywide.
4. Staffing headcounts do not account for differences between full-time and part-time employees or necessarily represent full-time equivalents.
5. Spending per linear foot does not account for local cost differences, district characteristics, or variations in service requirements.
6. Sanitation and public-safety ratios describe reported activity rather than service quality, productivity, or effectiveness.
7. Correlations describe statistical associations and should not be interpreted as causal relationships.
8. The digital subscriber-attendance analysis uses a restricted sample of 69 BIDs with positive reporting across four selected marketing variables. Excluding Times Square leaves 68 observations.
9. The G&A ratio analysis includes only 49 BIDs with complete reporting across all six expense categories.

## Project Resources

- **Jupyter Notebook:** [Explore the Python analysis](notebooks/)
- **Full HTML Report:** [Browse the complete analysis](reports/)
- **Visualizations:** [Explore project figures](figures/)
- **Personal Portfolio:** [juanfvargas.com](https://www.juanfvargas.com/)

---

*This project demonstrates the application of Python, exploratory data analysis, statistical methods, and data visualization to business and economic research.*
