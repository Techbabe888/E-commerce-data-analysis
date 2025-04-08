# E-commerce Data Analysis 
## Table of Contents  
1. [Project Overview](#project-overview)  
2. [Data Source](#data-source)  
3. [Tools Used](#tools-used)  
4. [Steps Taken](#steps-taken)  
   - [Data Cleaning](#data-cleaning)  
   - [Exploratory Data Analysis ](#exploratory-data-analysis)  
5. [Dashboard ](#dashboard)
6. [Key Insights and Findings ](#key-insights-and-findings)  
7. [Recommendations](#recommendations)  
8. [Conclusion](#conclusion)  
## Project Overview
This project analyzes an e-commerce dataset to understand customers behavior, products performance, and sales trends. The insights gained will help improve decision-making, enhance customer experience, and drive business growth.
## Data Source
- Kaggle
## Tools Used
- MySQL Server
- PowerBi
## Steps Taken
### Data Cleaning
- Data Importing and Inspection
- Handling missing values
- Standardization
- Checked for duplicates
   
### Exploratory Data Analysis
- Analyzed total revenue generated in each month
- Identified top-selling products
- Examined the most effective payment methods
- Determined which gender contributes to higher sales
- Analyzed login types
- Computed sum of sales in each product category using a window function
  ```sql
SELECT 
    Product_Category, 
    SUM(Sales) OVER (PARTITION BY Product_Category) AS Total_Sales 
FROM ecommerce_Data;
## Dashboard 

![ecommerce dashboard](ecommerce%20dashboard.PNG)

##  Download the Power BI File

> Note: To explore or interact with the report, open the `.pbix` file using Power BI Desktop.

👉 [Download Ecommerce report (.pbix)](Ecommerce%20report.pbix)

## Key insights and Findings
- Revenue Contribution by Gender: Male customers generated 55.15% of total revenue, while female customers accounted for 44.8%.
- Login Distribution: Existing members had the highest login activity, while first-time sign-ups and new users recorded 0.17% and 0.03%, respectively.
- Preferred Payment Method: Credit cards were the most used payment method, followed by money transfers, totaling 10,000 transactions.
- Top Product Categories: Fashion dominated sales with 55.62%, while Electronics recorded the lowest sales at 5.05%.
- Sales Performance by Month: November had the highest sales (877,881), followed by May, while January, February, and April performed poorly.
- Inactive Customers: A total of 39,000 inactive customers were recorded.

## Recommendations
### Revenue Contribution by Gender
- Ensure sufficient stock availability for high demand product categories to prevent shortage and meet customer needs
- Conduct customer surveys and feedback sessions to improve product offerings and overall shopping experience.
### Login Distribution
- Enhancing marketing strategies to attract first time and new users by offering by welcome discounts or incentives
- Improve user boarding experience by simplifying the sign up process and offering guided tutorial guide
- Levreage social media and referral programs to encourage new sign ups
### Preferred Payment Method
- Since credit cards are the most used payment method, ensure uninterrupted service by maintaining relaible transaction processing systems
- Offer incentive such as cashback, loyalty points, or discounts for digital payments to encourage more usage.
- Provide secure and user-friendly payment gateways to build customer trust in online transactions.
- Offer free Wi-Fi or ensure network reliability to avoid transaction failures due to poor connectivity.
### Top Product Categories
- With Fashion leading in sales, stay updated on industry trends, introduce seasonal collections, and offer styling recommendations to enhance customer experience.
- Since Electronics is underperforming, conduct customer surveys to identify preferred brands or products and adjust inventory accordingly.
- Implement targeted promotions or bundle deals on electronic products to boost sales.
### Sales Performance by Month
- With sales being low from January to April, implementing seasonal discounts, promotions, referral bonuses, and limited-time offers to attract more customers.
- Introduce flash sales, exclusive early-bird deals, and loyalty rewards to encourage repeat purchases.
### Inactive Customers
- Utilize the customer database to reach out to inactive customers through email, SMS, or personalized offers to re-engage them.
- Implement a win-back campaign, such as offering special discounts or loyalty rewards to encourage return purchases.
- Improve customer service follow-ups to address any past issues that may have led to inactivity.
### Customer Experience & Retention
- Introduce live chat or virtual assistance to provide real-time support for customer inquiries.
- Leverage customer loyalty programs, offering exclusive discounts or membership perks to retain existing customers.
## Conclusion
This e-commerce analysis has provided key insights into customer behavior, product performance, and sales trends. Findings indicate that Fashion is the leading product category, Credit Card is the most preferred payment method, and November records the highest sales. Additionally, low engagement from new users and a high number of inactive customers highlight opportunities for improvement.
I recommend ensuring sufficient stock availability for high-demand products, optimizing marketing strategies to attract and retain new users, and implementing customer re-engagement initiatives to drive business growth.
