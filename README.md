# 📊 Customer Segmentation & Spending Score Analysis Dashboard

## 📌 Project Overview

This project presents an end-to-end customer analytics solution built in Power BI to uncover patterns in customer spending behavior, purchasing frequency, income distribution, and loyalty performance.

The project consists of two interactive dashboards:

1. **Customer Segmentation Overview**
2. **Customer Spending Score Dashboard**

Together, these dashboards provide a comprehensive view of customer demographics, purchasing habits, spending behavior, and loyalty trends.

---

## 🎯 Business Problem

Businesses often collect large amounts of customer data but struggle to answer critical questions such as:

- Who are the most valuable customers?
- Which customer segments generate the most revenue?
- Does customer loyalty influence spending behavior?
- Which age groups spend the most?
- How does income impact purchasing patterns?
- Which product categories drive the highest sales?

This project aims to answer these questions through customer segmentation and spending behavior analysis.

---

# 🛠️ Tools & Technologies

| Tool | Purpose |
|--------|---------|
| Power BI | Dashboard Development & Visualization |
| Power Query | Data Cleaning & Transformation |
| DAX | KPI and Measure Creation |
| Excel | Data Storage & Preparation |

---

# 📂 Dataset Description

The dataset contains customer demographic and transactional information.

### Key Fields

| Field | Description |
|---------|-------------|
| Customer ID | Unique customer identifier |
| Age | Customer age |
| Gender | Customer gender |
| Income | Annual customer income |
| Spending Score | Customer spending rating |
| Membership Years | Customer tenure |
| Purchase Amount | Amount spent by customer |
| Purchase Frequency | Number of purchases made |
| Product Category | Product category purchased |

---

# 🧹 Data Cleaning & Preparation

Several preprocessing steps were performed to ensure data quality and consistency.

### Data Quality Checks

- Removed duplicate records
- Validated unique customer IDs
- Checked for missing values
- Standardized categorical fields
- Verified numerical data consistency

### Feature Engineering

#### Age Group Classification

Customers were grouped into the following age brackets:

- 18–27
- 28–37
- 38–47
- 48–57
- 58–69

#### Membership Segmentation

Customers were categorized based on membership duration:

- New Customers
- Mid-term Customers
- Loyal Customers

### DAX Measures Created

```DAX
Total Customers =
COUNT(Customer[ID])

Avg Age =
AVERAGE(Customer[Age])

Avg Income =
AVERAGE(Customer[Income])

Avg Purchase Amount =
AVERAGE(Customer[Purchase Amount])

Avg Spending Score =
AVERAGE(Customer[Spending Score])

Total Purchase Amount =
SUM(Customer[Purchase Amount])

Avg Purchase Frequency =
AVERAGE(Customer[Purchase Frequency])
```

---

# 📈 Dashboard 1: Customer Spending Score Dashboard

## Dashboard Objective

Analyze spending behavior across customer demographics and identify factors influencing spending scores.

### KPI Summary

| KPI | Value |
|--------|--------|
| Total Customers | 501K |
| Average Age | 44 |
| Average Purchase Amount | $492 |
| Average Spending Score | 50.69 |

### Insight

The customer base exhibits moderate spending behavior with a balanced distribution across demographic segments.

---

## Spending Score by Age Group

### Findings

| Age Group | Spending Score |
|------------|--------------|
| 58–69 | 12.1K |
| 38–47 | 10.6K |
| 28–37 | 9.8K |
| 48–57 | 9.5K |
| 18–27 | 8.7K |

### Business Insight

Customers aged **58–69 years** generate the highest spending scores, indicating that older customers are significantly more valuable from a spending perspective.

The **18–27 age group** contributes the lowest spending score, suggesting an opportunity to improve engagement among younger customers.

---

## Income Distribution by Spending Segment

### Findings

| Segment | Income Contribution |
|----------|------------------|
| High Spenders | 31M |
| Low Spenders | 31M |
| Medium Spenders | 27M |

### Business Insight

Income alone does not determine spending behavior.

The presence of high-income customers among low spenders highlights an opportunity for targeted marketing and personalized promotions.

---

## Spending Score by Gender

### Findings

| Gender | Percentage |
|----------|-----------|
| Male | 34.36% |
| Other | 33.41% |
| Female | 32.23% |

### Business Insight

Spending behavior is relatively balanced across genders.

Behavioral and loyalty segmentation may be more effective than demographic-based targeting.

---

## Last Purchase Amount by Product Category

### Findings

| Category | Purchase Amount |
|-----------|---------------|
| Electronics | 107K |
| Home & Garden | 104K |
| Sports | 101K |
| Groceries | 97K |
| Clothing | 83K |

### Business Insight

Electronics and Home & Garden products generate the highest purchase values, indicating strong customer demand in these categories.

Clothing contributes the lowest purchase value and may require promotional strategies to boost performance.

---

## Spending Trend by Membership Years

### Findings

Highest spending activity occurs at:

- 5 Years Membership
- 9 Years Membership

Lowest spending activity occurs at:

- 6 Years Membership

### Business Insight

Customer loyalty positively impacts spending behavior.

However, fluctuations after the fifth year indicate potential disengagement risks that require retention initiatives.

---

# 📈 Dashboard 2: Customer Segmentation Overview

## Dashboard Objective

Analyze customer composition, loyalty distribution, and revenue contribution across customer segments.

### KPI Summary

| KPI | Value |
|--------|--------|
| Total Purchase Amount | $492.35K |
| Average Income | $89K |
| Average Membership Years | 5 Years |
| Average Purchase Frequency | 26.60 |

---

## Customer Distribution by Membership Segment

### Findings

| Segment | Percentage |
|------------|----------|
| Loyal Customers | 48.2% |
| Mid-term Customers | 31.4% |
| New Customers | 20.4% |

### Business Insight

Nearly half of the customer base consists of loyal customers, indicating strong customer retention performance.

Loyal customers represent a critical asset for future revenue growth.

---

## Purchase Frequency by Age Group

### Findings

| Age Group | Purchase Frequency |
|------------|------------------|
| 58–69 | 234 |
| 38–47 | 199 |
| 48–57 | 196 |
| 28–37 | 186 |
| 18–27 | 185 |

### Business Insight

Older customers purchase more frequently than younger customers, reinforcing findings from the Spending Score Dashboard.

---

## Total Purchase Amount by Membership Group

### Findings

| Segment | Purchase Amount |
|------------|----------------|
| Loyal Customers | $230K |
| Mid-term Customers | $150K |
| New Customers | $100K |

### Business Insight

Revenue contribution increases significantly as customers become more loyal.

Customer retention directly impacts business profitability.

---

## Trend of Purchase Frequency

### Findings

Peak purchase frequency occurs during:

- Year 5 Membership

Lowest purchase frequency occurs during:

- Year 8 Membership

### Business Insight

Customers are most engaged during the middle stages of their lifecycle.

Organizations should implement retention campaigns before engagement begins to decline.

---

## Purchase Frequency Distribution by Income

### Findings

| Segment | Value |
|----------|--------|
| Medium Frequency | 32.1M |
| High Frequency | 29.9M |
| Low Frequency | 26.6M |

### Business Insight

Medium-frequency customers represent the largest purchasing group and offer significant growth potential.

Converting these customers into high-frequency buyers could substantially increase revenue.

---

# 🔍 Executive Summary of Findings

### Key Finding 1

Customer loyalty is the strongest predictor of revenue contribution.

### Key Finding 2

Customers aged 58–69 consistently outperform all other age groups in spending score and purchase frequency.

### Key Finding 3

Electronics, Home & Garden, and Sports categories generate the highest customer spending.

### Key Finding 4

Income does not always translate into higher spending behavior.

### Key Finding 5

Customer engagement peaks around the fifth year of membership.

---

# 💡 Strategic Recommendations

## 1. Strengthen Customer Loyalty Programs

- Introduce VIP membership tiers
- Reward repeat purchases
- Offer exclusive benefits to long-term customers

### Expected Outcome

Higher retention and increased customer lifetime value.

---

## 2. Improve Engagement Among Younger Customers

- Launch personalized promotions
- Offer student and early-career discounts
- Increase social media marketing efforts

### Expected Outcome

Increased spending and purchase frequency among younger demographics.

---

## 3. Target High-Income Low-Spending Customers

- Create personalized product recommendations
- Offer premium bundles
- Implement targeted email campaigns

### Expected Outcome

Improved conversion and higher average spending.

---

## 4. Maximize High-Performing Product Categories

Focus on:

- Electronics
- Home & Garden
- Sports

through cross-selling and upselling strategies.

### Expected Outcome

Revenue growth and increased basket size.

---

## 5. Re-engage Mid-Lifecycle Customers

Implement retention campaigns between years 5–8.

Examples:

- Anniversary rewards
- Loyalty bonuses
- Exclusive promotions

### Expected Outcome

Reduced churn and improved customer retention.

---

# 🚀 Skills Demonstrated

This project demonstrates proficiency in:

- Data Cleaning
- Data Transformation
- Customer Segmentation
- Business Intelligence
- Data Storytelling
- Dashboard Design
- KPI Development
- DAX Measures
- Power Query
- Data Visualization
- Business Insights Generation

---

# 📷 Dashboard Preview
# 📊 Customer Segmentation & Spending Score Analysis
<img width="508" height="313" alt="Screenshot 2026-06-02 034610" src="https://github.com/user-attachments/assets/6dc8e509-f4ce-4be3-b052-df6a864a1b3c" />


![Combined Dashboard](Images/Combined_Dashboard.png)

### Customer Segmentation Overview

![Customer Segmentation Dashboard](/>ges/customer_segmentation_dashboard.png)<img width="545" height="333" alt="Screenshot 2026-06-02 034817" src="https://github.com/user-attachments/assets/bb248f69-c497-4215-86b1-e85793ff01ed" />



### Customer Spending Score Dashboard

![Customer Spending Dashboard](images/<img width="545" height="332" alt="Screenshot 2026-06-02 033859" src="https://github.com/user-attachments/assets/01afdb04-da92-4f56-9ec9-5888e0bd7193" />
customer_spending_dashboard.png)

---

# 👤 Author

**Adaobi Lilian Amuchuoka**

Aspiring Data Analyst | Power BI Developer

### Connect With Me

- LinkedIn: www.linkedin.com/in/amuchuoka-adaobi-lilian-1492492a6
- GitHub: github.com/yourusername
- Email: amuchuokaadaobi@gmail.com<



---
⭐ If you found this project interesting, feel free to star the repository and connect with me.
