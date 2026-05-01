# 🛒 Retail Customer Retention Analytics – Walmart

## 📌 Project Overview
With increasing competition from Amazon, Target, and other retailers, retaining customers has become a critical challenge for Walmart. While vast customer data is available, existing reporting lacks analytical depth.
This project focuses on building an **interactive Customer Retention Analytics Dashboard in Power BI** to uncover insights and drive data-backed retention strategies.

---

## 🎯 Objectives
- Consolidate customer demographics, transactions, store, and loyalty data  
- Enable segmentation of customers (high-value, repeat, churned)  
- Analyze churn behavior and retention patterns  
- Provide actionable recommendations to improve retention and engagement  

---

## 📂 Dataset Description

### 1. Customer_Demographics
- Customer_ID, Age, Gender, Region, Income_Level  
- Membership_Since, Preferred_Channel  

### 2. Customer_Transactions
- Transaction_ID, Customer_ID, Store_ID  
- Product_Category, Transaction_Date  
- Amount, Promotion_Applied  

### 3. Store_Locations
- Store_ID, Store_Type, Region, Opening_Year  

### 4. Loyalty_Program
- Customer_ID, Loyalty_Tier  
- Points_Earned, Points_Redeemed  

### 5. Churn_Labelled_Customers
- Customer_ID, Last_Purchase_Date  
- Churn_Flag, Churn_Reason  

---

## 🧹 Data Cleaning & Preparation
- Handled missing values and duplicates in Power Query  
- Ensured correct data types across all tables  
- Created calculated columns:
  - `Membership_Duration`
  - `Transaction_Year`
  - `Transaction_Month`

---

## 🧩 Data Model
- One-to-Many Relationships:
  - Customer → Transactions  
  - Customer → Loyalty Program  
  - Customer → Churn Table  
- Many-to-One:
  - Transactions → Store  

---

## 📊 Key Metrics & KPIs

### 🔻 Churn Analysis
- **Churn Rate:** 49.7%  
- Churn segmented by:
  - Region  
  - Income Level  
  - Channel (Store vs Online)  
  - Loyalty Tier  

- Funnel Analysis:
  - Total Customers → Repeat Customers → Churned  
  - **300 → 251 → 149**

---

### 🔁 Repeat Purchase Analysis
- Customer Segmentation:
  - Low: 0–3 purchases  
  - Mid: 4–8 purchases  
  - High: 9+ purchases  

- **Average Purchase Frequency:** 3.4  

- Most purchased categories:
  - Groceries (Basic, Plus, Premium)  
  - Apparel (Elite Tier)  

---

### 🎁 Promotion & Loyalty Insights
- 49% transactions used promotions  
- Avg purchase with promotion ≈ without promotion  
  → Promotions are **not effective**

- Higher churn observed in:
  - Elite & Plus tiers  

---

### 🏬 Store & Channel Insights
- Higher churn observed in:
  - Neighborhood Market  
  - Supercenter  

- Better retention in:
  - Newer stores  

- Online channel users show:
  - Higher churn tendency  

---

### 💰 Customer Lifetime Value (CLV)
- **CLV = Total Spend / Membership Duration**
- Average CLV: **305.5/year**

Key insights:
- Basic tier has highest avg CLV  
- Central region has highest CLV  
- Negative correlation:
  - More recent purchase → Higher CLV  

---

## 📈 Dashboard Overview

### 📄 Page 1: KPI Dashboard
- Churn Rate  
- CLV  
- Repeat Customers
- Regional performance  

### 📄 Page 2: Loyalty & Promotion Impact
- Churn by loyalty tier  
- Points earned vs redeemed  
- Promotion effectiveness  

### 📄 Page 3: Store & Channel Insights
- Churn by store type  
- Avg transaction value  
- Channel comparison  

### 📄 Page 4: Customer Segmentation
- High-value customers  
- Purchase frequency accross age groups  
- CLV segmentation  

---

## 🔍 Key Insights

- Nearly **50% customers are churned**, indicating retention challenges  
- Promotions do **not significantly impact spending behavior**  
- **Elite and Plus customers show higher churn**, despite being premium users  
- Online channel users are more likely to churn than store users  
- **Customer recency is strongly linked to CLV**  

---

## 🚀 Recommendations

### 🥇 1. Focus on High-Value At-Risk Customers
- Target customers with high CLV and inactivity signals  
- Launch personalized re-engagement campaigns  
- Use inactivity triggers (30–60 days)

---

### 🥈 2. Improve Underperforming Channels
- Optimize online experience (UX, delivery, recommendations)  
- Enhance in-store experience for high-churn stores  
- Leverage high-performing stores (e.g., Sam’s Club)  

---

### 🥉 3. Strengthen Loyalty Program Engagement
- Introduce behavior-based rewards  
- Improve redemption experience  
- Offer tier-based exclusive benefits  
- Shift from generic promotions → personalized incentives  

---

## 🛠 Tools & Technologies
- Power BI  
- DAX  
- Power Query  
- Data Modeling  

---

## 📽️ Project Demo
*(Add your video link here)*

---

## 📌 Conclusion
This project demonstrates how data-driven insights can help retail businesses:
- Reduce churn  
- Improve customer engagement  
- Maximize lifetime value  

By combining **customer segmentation, behavioral analysis, and business strategy**, this dashboard provides actionable insights for retention-focused decision-making.

---
