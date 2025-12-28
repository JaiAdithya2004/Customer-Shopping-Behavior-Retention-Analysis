# 🛍️ Customer Shopping Behavior & Retention Analysis

A comprehensive data analysis project examining 3,900 customer transactions to uncover shopping patterns, customer segments, and revenue drivers for strategic business insights.

## 📊 Project Overview

This project analyzes customer shopping behavior across multiple dimensions including demographics, purchase patterns, product preferences, and subscription status to guide data-driven business decisions.

## 🎯 Key Features

- **Customer Segmentation**: Classification into New, Returning, and Loyal customer groups
- **Revenue Analysis**: Breakdown by gender, age groups, and subscription status
- **Product Insights**: Top-rated items and category performance metrics
- **Behavioral Patterns**: Discount usage, shipping preferences, and purchase frequency
- **Interactive Dashboard**: Power BI visualization for stakeholder insights

## 🗂️ Dataset Summary

- **Records**: 3,900 transactions
- **Features**: 18 columns including:
  - Demographics (Age, Gender, Location)
  - Purchase Details (Item, Category, Amount, Season)
  - Behavior Metrics (Discounts, Reviews, Purchase Frequency)

## 🛠️ Tech Stack

- **Python**: Data cleaning, feature engineering, and preprocessing
- **PostgreSQL**: Business logic queries and advanced analytics
- **Power BI**: Interactive dashboard and visualizations
- **Libraries**: pandas, psycopg2, numpy

## 🔍 Analysis Workflow

### 1. Data Preparation (Python)
- Imported and explored dataset structure
- Handled 37 missing values in Review Rating using median imputation
- Standardized column names to snake_case
- Engineered features: `age_group`, `purchase_frequency_days`
- Validated and removed redundant columns
- Loaded cleaned data into PostgreSQL

### 2. Business Analysis (SQL)
Executed 10 strategic queries:
- Revenue comparisons by gender and subscription status
- High-spending discount user identification
- Product performance by ratings and category
- Shipping type purchase behavior analysis
- Customer segmentation based on purchase history
- Discount dependency analysis by product
- Age group revenue contribution

### 3. Visualization (Power BI)
Created interactive dashboard featuring:
- Revenue metrics and trends
- Customer segmentation distributions
- Product performance rankings
- Demographic insights

## 💡 Key Insights & Recommendations

### Business Strategies
1. **Subscription Growth**: Promote exclusive benefits to convert high-frequency buyers
2. **Loyalty Programs**: Reward repeat customers to drive retention
3. **Discount Optimization**: Balance promotional sales with margin protection
4. **Product Positioning**: Highlight top-rated items in marketing campaigns
5. **Targeted Marketing**: Focus on high-revenue age segments and express shipping users

## 📁 Repository Structure

```
├── data/
│   ├── raw/                    # Original dataset
│   └── cleaned/                # Processed data
├── scripts/
│   ├── data_cleaning.py        # Python preprocessing
│   └── analysis_queries.sql    # PostgreSQL queries
├── dashboard/
│   └── shopping_analysis.pbix  # Power BI dashboard
├── reports/
│   └── analysis_report.pdf     # Detailed findings
└── README.md
```

## 🚀 Getting Started

### Prerequisites
```bash
Python 3.8+
PostgreSQL 12+
Power BI Desktop
```

### Installation
```bash
# Clone repository
git clone https://github.com/yourusername/customer-shopping-analysis.git

# Install Python dependencies
pip install -r requirements.txt

# Set up PostgreSQL database
psql -U postgres -f scripts/setup_database.sql
```

### Usage
```bash
# Run data cleaning pipeline
python scripts/data_cleaning.py

# Execute SQL analysis
psql -U postgres -d shopping_db -f scripts/analysis_queries.sql

# Open Power BI dashboard
# File -> Open -> dashboard/shopping_analysis.pbix
```

## 📈 Results

- Identified customer segments contributing to 75% of total revenue
- Discovered 23% higher spending among subscribers vs. non-subscribers
- Mapped discount effectiveness across product categories
- Revealed age group and shipping preference correlations

## Dashboard


<img width="988" height="553" alt="Screenshot 2025-12-27 193347" src="https://github.com/user-attachments/assets/20dfccc8-382f-459a-866e-5902bcf6f55e" />
