# Task 6 – Netflix Business Insights Dashboard

## Project Overview

This project focuses on analyzing Netflix catalogue data and developing an interactive business insights dashboard using Python and Plotly.

The objective was to understand content distribution, identify catalogue trends, perform basic predictive analysis, and communicate findings through interactive visualizations.

## Objectives

- Analyze Movies and TV Shows distribution.
- Identify top countries and genres.
- Examine content rating patterns.
- Analyze yearly content additions.
- Develop and evaluate a Linear Regression model.
- Build an interactive business insights dashboard.
- Generate data-driven business recommendations.

## Tools & Technologies

- Python
- Jupyter Notebook
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Plotly
- Scikit-learn

## Dataset

The project uses the cleaned Netflix dataset containing 8,790 records and 12 columns.

The dataset includes information about content type, country, release year, genre, ratings, and dates added.

## Key Business Metrics

| Metric | Result |
|---|---:|
| Total Titles | 8,790 |
| Movies | 6,126 |
| TV Shows | 2,664 |
| Movie Percentage | 69.69% |
| TV Show Percentage | 30.31% |
| Unique Country Entries | 86 |
| Unique Genre Combinations | 513 |
| Average Release Year | 2014.18 |

Note: Country and genre counts refer to distinct combined entries in the original columns, not individual countries or genres.

## Analysis Performed

1. Prepared the cleaned dataset for business analysis.
2. Created time-based features from the date added column.
3. Analyzed yearly content additions.
4. Explored country-wise content distribution.
5. Identified leading genre categories.
6. Examined content rating distributions.
7. Compared Movies and TV Shows across countries.

## Predictive Trend Analysis

A Linear Regression model was trained using yearly content additions.

Training data: Years up to 2018.

Testing data: 2019 onwards.

| Evaluation Metric | Result |
|---|---:|
| MAE | 572.74 |
| RMSE | 657.78 |
| R² | -8.009 |

The model achieved lower MAE and RMSE than the training-mean baseline, but its negative R² indicates weak predictive performance on the test period.

## Interactive Dashboard

The Plotly dashboard includes:

- Movies vs TV Shows distribution
- Yearly content additions
- Top 10 countries
- Top 10 genres

Additional interactive charts were developed for content type by country and content ratings.

### Dashboard File

[Open Interactive Netflix Business Insights Dashboard](Netflix_Business_Insights_Dashboard.html)

## Business Recommendations

1. Evaluate opportunities to diversify Movies and TV Shows based on audience demand.
2. Explore regional content strategies using country-wise catalogue representation and audience engagement data.
3. Study genre performance alongside actual viewing behaviour before making content investment decisions.
4. Investigate the decline in yearly additions after 2019.
5. Explore additional forecasting methods and features to improve predictive performance.

## Limitations

The dataset contains catalogue metadata but does not include subscriber numbers, viewing hours, revenue, or customer engagement information.

Therefore, business recommendations are exploratory and should be validated using actual business performance data.

## Key Learning Outcomes

- Business-oriented data analysis
- KPI development
- Data aggregation and visualization
- Time-based analysis
- Linear Regression
- Model evaluation
- Interactive dashboard development
- Business recommendations and reporting

## Project File

- `Task 6.ipynb` – Jupyter Notebook containing the analysis and dashboard development.
- `Netflix_Business_Insights_Dashboard.html` – Interactive dashboard.

