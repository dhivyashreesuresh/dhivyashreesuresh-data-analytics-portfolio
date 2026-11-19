# Retail Sales Analysis Using Python

## Project Overview

This project explores an online retail transaction dataset to identify sales trends, top-performing products, geographical revenue distribution and monthly revenue patterns.

Using Python and Pandas, I performed data cleaning, exploratory data analysis, feature engineering and data visualization to derive actionable business insights.

## Objectives

- Understand the structure and quality of retail transaction data.
- Identify and investigate missing values, duplicates and unusual transactions.
- Calculate revenue and key sales performance metrics.
- Identify top-performing products and international markets.
- Analyze monthly revenue trends.
- Present findings through visualizations and business recommendations.

## Tools and Technologies

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Google Colab

## Dataset

**Source:** [UCI Machine Learning Repository – Online Retail Dataset](https://archive.ics.uci.edu/dataset/352/online+retail)

The dataset contains online retail transactions recorded between December 2010 and December 2011.

It includes invoice numbers, product codes, product descriptions, quantities, invoice dates, unit prices, customer IDs and countries.

## Project Workflow

1. **Data Loading and Exploration:** Imported the dataset and examined its dimensions, columns and statistical summaries.
2. **Data Quality Assessment:** Investigated missing values, duplicate records, cancelled invoices and unusual transaction values.
3. **Data Cleaning:** Removed exact duplicate records from a working copy and created an analytical subset of positive-quantity, positive-price transactions.
4. **Feature Engineering:** Calculated revenue for each transaction line using Quantity × UnitPrice.
5. **Exploratory Data Analysis:** Analyzed overall revenue, average order value, product performance, country performance and monthly trends.
6. **Data Visualization:** Created charts to communicate product, geographical and monthly revenue patterns.

## Key Findings

| Metric | Result |
|---|---:|
| Original transaction records | 541,909 |
| Records after exact duplicate removal | 536,641 |
| Selected positive-sales records | 524,878 |
| Total gross revenue | £10,642,110.80 |
| Unique invoices | 19,960 |
| Average order value | £533.17 |
| UK revenue contribution | 84.59% |

### Product Performance
- Identified the highest-revenue product entries.
- Found that some product descriptions were associated with multiple stock codes.
- Retained both stock codes and descriptions for more granular product analysis.

### Geographical Performance
- The United Kingdom contributed approximately 84.59% of gross revenue.
- The Netherlands, EIRE, Germany and France were among the leading international markets.
- International revenue was concentrated among a relatively small number of countries.

### Monthly Revenue Trends
- November 2011 recorded the highest monthly revenue at £1,503,866.78.
- February 2011 recorded the lowest monthly revenue at £522,545.56.
- Revenue increased significantly between September and November.
- December 2011 data was incomplete, with transactions recorded only through December 9.

## Business Recommendations

- Explore growth opportunities in international markets to diversify revenue.
- Prioritize inventory planning for high-performing products.
- Use historical sales trends to prepare for seasonal demand.
- Monitor geographical revenue concentration and market performance.

## Important Data Considerations

- Exact duplicate records were removed from a working copy. Identical transaction lines cannot always be confirmed as accidental duplicates because the dataset does not provide a unique transaction-line identifier.
- The positive-sales subset includes records with Quantity greater than zero and UnitPrice greater than zero. Returns, cancellations, zero-price transactions and negative-price adjustments were excluded from this gross revenue calculation.
- Therefore, the reported revenue is not net revenue or profit.
- Some high-revenue entries, such as postage and manual adjustments, may not represent physical products.
- Missing customer IDs were retained, but this limits customer-level analysis.
- December 2011 is incomplete and should not be compared directly with full months.

## Conclusion

This project demonstrates the use of Python for practical retail data analysis, from data quality assessment and cleaning to feature engineering, visualization and business interpretation.

The findings highlight product performance, geographical revenue concentration and monthly sales patterns that can support data-informed business decisions.
