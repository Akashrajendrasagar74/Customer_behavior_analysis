# Customer_behavior_analysis
Customer Shopping Behavior Analysis using Python, SQL, and Power BI. Analyzed 3,900+ transactions to uncover spending patterns, customer segments, product performance, and subscription behavior. Built an interactive dashboard and delivered data-driven business recommendations.
# Project Overview
This project analyzes transactional data from 3,900 purchases across various product categories to uncover deep insights into customer spending patterns, segmentation, and preferences. By leveraging a combination of Python, SQL, and Power BI, the analysis provides actionable data to guide strategic business decisions regarding subscription models and marketing efforts.
                             
# Dataset Summary
  The dataset contains 3,900 rows and 18 columns, focusing on key retail metrics:
   •	Customer Demographics: Age, Gender, Location, and Subscription Status.
   •	Purchase Details: Items, Categories, Purchase Amount, Size, Color, and Season.
   •	Behavioral Metrics: Discounts, Promo Codes, Previous Purchases, Purchase Frequency, and Review Ratings.

# Data Pipeline
1. Exploratory Data Analysis (EDA) & Cleaning (Python)
  Data preparation was performed using Python (Pandas) to ensure data integrity:
   •	Initial Exploration: Used df.info() and describe() to understand data structure and summary statistics.
   •	Handling Missing Values: Identified 37 missing values in the Review Rating column and imputed them using the median rating of each product category.
   •	Feature Engineering: * Binned ages into an age_group column.
   •	Redundancy Check: Dropped the promo_code_used column as it was redundant with discount_applied.
   •	Database Integration: The cleaned data was loaded into a PostgreSQL database for advanced querying.
2. Structured Analysis (SQL)
  The following business questions were addressed using SQL queries:
   •	Revenue by Gender: Male customers contributed significantly more revenue ($157,890) compared to female customers ($75,191).
   •	Subscription Impact: While non-subscribers generate more total revenue due to volume, both groups maintain a similar average spend (approx. $59).
   •	Customer Segmentation: Classified users into Loyal (3,116), Returning (701), and New (83) segments based on purchase history.
   •	Top Products: Identified top-rated items like Gloves (3.86) and Sandals (3.84).
3. Interactive Dashboard (Power BI)
  A visual dashboard was developed to provide a high-level overview of key performance indicators (KPIs):
   •	KPI Cards: Total Customers (3.9K), Average Purchase Amount ($59.76), and Average Review Rating (3.75).
   •	Visualizations:
    1.	Revenue by Category: Clothing and Accessories are the leading revenue drivers.
    2.	Customer Mix: 27% of customers are subscribers, while 73% are not.
    3.	Demographic Trends: Revenue distribution analyzed by age groups (Young Adult, Middle-aged, Adult, and Senior).

# Business Recommendations
  •	Boost Subscriptions: Launch targeted campaigns to convert the 73% of non-subscribers by promoting exclusive benefits.
  •	Loyalty Programs: Focus on moving "Returning" customers into the "Loyal" segment through reward systems.
  •	Marketing Focus: Prioritize marketing efforts toward Young Adults, who represent the highest revenue-contributing age group ($62,143).
  •	Inventory Optimization: Highlight top-rated products like Gloves and Sandals in promotional materials to drive sales.

