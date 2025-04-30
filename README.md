# Supermarket Sales Analysis & Optimization

## Project Overview

This project analyzes transaction data from City Mall Holdings, a supermarket chain operating in Myanmar, to address key business challenges around customer engagement, inventory management, and payment method optimization. The analysis was conducted on 1,000 sales records spanning three months (January-March 2019) across three branches in Yangon, Mandalay, and Naypyitaw.

## Key Business Problems Addressed

1. **Customer Segmentation**: Identifying distinct customer segments to develop targeted marketing strategies
2. **Time Series Analysis**: Analyzing sales patterns to optimize inventory management
3. **Payment Method Analysis**: Evaluating payment method utilization across different customer segments and branches

## Data Description

The dataset contains 1,000 transaction records with 17 variables including:

- **Invoice ID**: Unique identifier for each transaction
- **Branch/City**: Location information (Yangon, Mandalay, Naypyitaw)
- **Customer Demographics**: Type (Member/Normal) and Gender
- **Product Details**: Product line, unit price, quantity
- **Financial Information**: Tax, total amount, COGS, gross margin
- **Transaction Context**: Date, time, payment method
- **Customer Feedback**: Satisfaction rating

## Methodology

### Data Preprocessing
- Data quality checks (duplicates, missing values)
- Date/time formatting and feature engineering
- Creation of time-based features for analysis

### Customer Segmentation
- K-Means clustering on transaction characteristics and demographics
- Optimal cluster determination using Elbow Method and Silhouette Analysis
- Creation of five distinct customer segments

### Time Series Analysis
- Daily sales aggregation for key product lines
- Trend and seasonality visualization
- Time series decomposition into trend, seasonal, and residual components

### Payment Method Analysis
- Comparative statistics across payment methods
- Segmented analysis by location and customer type
- Value association with different payment methods

## Key Findings

### Customer Segments
Five distinct customer segments were identified:
1. **High-Value Members**: Highest average spending and quantity, predominantly members
2. **High Spend/Quantity - Normal Focus**: High average spending but with more non-member customers
3. **Low-Value Convenience**: Lowest spending and quantity, likely impulse purchases
4. **Mid-Value Members (2 segments)**: Core member base with moderate spending patterns

### Inventory Insights
- Significant daily sales volatility across product lines
- Clear weekly seasonality patterns, particularly in Food & Beverages
- Potential stockout periods identified in key product categories

### Payment Method Patterns
- E-wallet and Cash are most frequently used (34.5% and 34.4%)
- Cash transactions have highest average value (326.18 MMK)
- Regional preferences vary (e.g., Naypyitaw prefers Cash, Yangon favors E-wallet)
- Members show higher preference for Credit Card payments

## Recommendations

### Customer Engagement
1. Implement tiered loyalty program for high-value members
2. Target high-spending non-members with membership conversion incentives
3. Use strategic product placement to increase basket size for low-value segments
4. Maintain consistent communication with core member segments

### Inventory Optimization
1. Adjust ordering schedules based on weekly seasonality patterns
2. Investigate identified stockout periods to determine root causes
3. Implement safety stock for top SKUs in categories with stockout risk

### Payment Method Optimization
1. Analyze processing costs for each payment method
2. Customize payment operations by branch to match local preferences
3. Consider loyalty incentives for preferred payment methods

## Tools & Technologies
- **Environment**: Google Colab
- **Libraries**: Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn, Statsmodels, Yellowbrick

## Project Structure
- Data preprocessing and cleaning
- Exploratory data analysis and descriptive statistics
- Customer segmentation using K-means clustering
- Time series analysis for inventory patterns
- Payment method utilization analysis
- Business recommendations based on findings

## Source
- Dataset: Supermarket sales dataset (publicly available)
- Analysis: [Google Colab Notebook](link-to-notebook)

---
*This project was completed as part of the BDM capstone Project for the IITM Online BS Degree Program.*

