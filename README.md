Customer Shopping Behavior Analysis
A comprehensive data analysis project examining customer shopping patterns using transactional data from 3,900 purchases across various product categories. This project combines Python data processing, SQL analytics, and Power BI visualization to uncover actionable business insights.
📊 Project Overview
This analysis explores customer spending patterns, product preferences, and subscription behavior to guide strategic business decisions. The project demonstrates end-to-end data analysis skills including data cleaning, SQL queries, and interactive dashboard development.
🎯 Key Objectives
•	Analyze customer spending patterns across demographics
•	Identify high-value customer segments
•	Evaluate product performance and ratings
•	Assess discount effectiveness
•	Compare subscription vs. non-subscription behavior
•	Generate actionable business recommendations
📁 Dataset Summary
•	Total Records: 3,900 purchases
•	Features: 18 columns
•	Key Data Points: 
o	Customer demographics (Age, Gender, Location, Subscription Status)
o	Purchase details (Item, Category, Amount, Season, Size, Color)
o	Shopping behavior (Discounts, Previous Purchases, Frequency, Review Ratings, Shipping Type)
•	Missing Data: 37 values in Review Rating column (handled via median imputation)
🛠️ Technologies Used
•	Python: Data cleaning, preprocessing, and feature engineering 
o	pandas
o	numpy
o	 (MYSQL integration)
•	SQL: MYSQL for business analytics queries
•	Power BI: Interactive dashboard and data visualization
📈 Analysis Workflow
1. Data Preparation (Python)
# Key steps performed:
- Data loading and initial exploration
- Missing data handling (median imputation by category)
- Column standardization (snake_case naming)
- Feature engineering (age groups, purchase frequency)
- Data consistency checks
- MYSQL database integration
Feature Engineering:
•	Created age_group column by binning customer ages
•	Generated purchase_frequency_days from purchase data
•	Removed redundant promo_code_used column
2. Business Analytics (SQL)
Executed 10 key business queries in MYSQL:
1.	Revenue by Gender - Compared spending patterns between male and female customers
2.	High-Spending Discount Users - Identified customers using discounts while spending above average
3.	Top 5 Products by Rating - Found highest-rated products (Gloves: 3.86, Sandals: 3.84, Boots: 3.82)
4.	Shipping Type Comparison - Analyzed Express vs. Standard shipping preferences
5.	Subscribers vs. Non-Subscribers - Compared average spend and revenue contribution
6.	Discount-Dependent Products - Identified products with highest discount usage rates
7.	Customer Segmentation - Classified customers as New, Returning, or Loyal
8.	Top 3 Products per Category - Listed best-sellers within each product category
9.	Repeat Buyers & Subscriptions - Analyzed subscription likelihood among frequent buyers
10.	Revenue by Age Group - Calculated revenue contribution across age segments
3. Data Visualization (Power BI)
Created an interactive dashboard featuring:
•	Key metrics: Customer count, average purchase amount, average review rating
•	Subscription status distribution
•	Revenue and sales breakdowns by category
•	Age group analysis
•	Category performance comparisons
•	Interactive filters for detailed exploration
🔍 Key Findings
Customer Segmentation
•	Loyal Customers: 3,116 (79.9%)
•	Returning Customers: 701 (18.0%)
•	New Customers: 83 (2.1%)
Revenue Insights
•	Male customers generated $157,890 in revenue
•	Female customers generated $75,191 in revenue
•	Young Adults contributed the highest total revenue ($62,143)
•	Average purchase amounts remained consistent across age groups (~$59-60)
Product Performance
•	Top-rated products: Gloves (3.86), Sandals (3.84), Boots (3.82), Hat (3.80), Skirt (3.78)
•	Most purchased items vary by category: 
o	Accessories: Jewelry, Sunglasses, Belt
o	Clothing: Blouse, Pants, Shirt
o	Footwear: Sandals, Shoes, Sneakers
o	Outerwear: Jacket, Coat
Discount Analysis
•	839 customers used discounts but still spent above average
•	Highest discount-dependent products: Hat (50%), Sneakers (49.66%), Coat (49.07%)
Subscription Behavior
•	Subscribers: 1,053 customers (27%), generating $62,645 in revenue
•	Non-subscribers: 2,847 customers (73%), generating $170,436 in revenue
•	Average spend nearly identical between groups (~$59)
Shipping Preferences
•	Express shipping: Average purchase $60.48
•	Standard shipping: Average purchase $58.46
💡 Business Recommendations
1.	Boost Subscription Programs
o	Promote exclusive benefits to increase subscription rates
o	Target the 73% non-subscriber base with value propositions
2.	Implement Customer Loyalty Programs
o	Reward repeat buyers to strengthen the loyal customer segment
o	Create pathways to move Returning customers to Loyal status
3.	Optimize Discount Strategy
o	Review discount policies to balance sales volume with profit margins
o	Focus discounts on products with lower natural demand
o	Maintain premium positioning for high-rated products
4.	Strategic Product Positioning
o	Highlight top-rated products (Gloves, Sandals, Boots) in marketing campaigns
o	Feature category best-sellers prominently
5.	Targeted Marketing Campaigns
o	Focus efforts on high-revenue age groups (Young Adults)
o	Target Express shipping users with premium product offerings
o	Develop gender-specific marketing strategies based on spending patterns
📂 Repository Structure
customer-shopping-analysis/
│
├── data/
│   └── raw_data.csv                 # Original dataset
│
├── notebooks/
│   ├── data_cleaning.ipynb          # Python data preprocessing
│   └── exploratory_analysis.ipynb   # Initial EDA
│
├── sql/
│   └── business_queries.sql         # All SQL analysis queries
│
├── dashboards/
│   └── customer_behavior.pbix       # Power BI dashboard
│
├── reports/
│   └── analysis_report.pdf          # Detailed findings report
│
└── README.md                        # Project documentation
🚀 Getting Started
Prerequisites
Python 3.8+
MYSQL 9+
Power BI Desktop
Installation
1.	Clone the repository
git clone https://github.com/sanket01-lang/Customer-Shopping-Behavior-Analysis
2.	Install Python dependencies
pip install pandas numpy psycopg2-binary
3.	Set up MYSQL database
CREATE DATABASE shopping_analysis;
4.	Run the data pipeline
python scripts/data_pipeline.py
5.	Execute SQL queries
psql -d shopping_analysis -f sql/business_queries.sql
6.	Open Power BI dashboard
Open dashboards/customer_behavior_dashboard.pbix in Power BI Desktop
📊 Dashboard Preview
The Power BI dashboard includes:
•	Interactive filters for Subscription Status, Gender, Category, and Shipping Type
•	KPI cards showing total customers, average purchase amount, and average rating
•	Visualizations for subscription distribution, revenue by category, sales by category
•	Age group analysis for both revenue and sales
•	Dynamic filtering capabilities for detailed insights
🤝 Contributing
Contributions are welcome! Please feel free to submit a Pull Request.
👤 Author
Sanket Nagdive
•	GitHub: @sanket01-lang
🙏 Acknowledgments
•	Inspiration and guidance from data analysis community
________________________________________
⭐ If you found this project helpful, please consider giving it a star!

