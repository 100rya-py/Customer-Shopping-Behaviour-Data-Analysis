# 🛍️ Customer Shopping Behavior Analysis

## 👋 Welcome!
Hi there! Welcome to my end-to-end data analysis project.

Have you ever wondered what really drives a customer to hit that "Buy" button? In this project, I analyzed 3,900 purchase records to uncover the hidden patterns behind customer spending, subscription habits, and product preferences.

I didn't just want to crunch numbers; I wanted to provide actionable advice. So, I took this project through the entire data lifecycle: **Cleaning in Python ➡️ Querying in SQL ➡️ Visualizing in Power BI.**

---
## 📊 Project Presentation
View the detailed business insights and findings in the presentation:
[📄 View Project PPT](https://github.com/100rya-py/Customer-Shopping-Behaviour-Data-Analysis/blob/main/Customer-Shopping-Behavior-Analysis%20Presentation.pdf)

## 🛠️ The Tech Stack
* **Python (Pandas):** For data cleaning, feature engineering, and preparation.
* **SQL (MySQL Workbench):** For solving critical business questions and data exploration.
* **Power BI:** For building the interactive dashboard.

---

## 🔄 Step 1: Data Cleaning & Prep (Python)
Before I could find any insights, I had to make sure the data was trustworthy. Using a Jupyter Notebook, I performed the following steps:
* **Handling Missing Data:** I found missing values in the `Review Rating` column and filled them intelligently using the median rating of each specific product category to avoid bias.
* **Feature Engineering:** I created new columns like `age_group` (classifying users into Young Adult, Senior, etc.) and converted purchase frequency into numeric days for better analysis.
* **Cleaning Up:** I noticed `discount_applied` and `promo_code_used` were providing the same information, so I removed the redundant column to keep the dataset lean.

---

## 🔍 Step 2: Solving Business Problems (SQL)
Once the data was clean, I moved it into a SQL database to answer the tough questions. Here is what I looked into:
* **Revenue Analysis:** I compared revenue between genders and found that Male customers generated significantly higher total revenue ($157k) compared to Female customers ($75k).
* **Shipping & Spending:** I analyzed if faster shipping equals higher spending. Surprisingly, the average spend for **Express Shipping ($60.48)** was only slightly higher than **Standard Shipping ($58.46)**.
* **The Discount Hunters:** I identified a segment of 839 customers who used discounts but still managed to spend *above* the average purchase amount—a goldmine for marketing!.
* **Product Ratings:** I ranked the top 5 highest-rated items, with Gloves and Sandals leading the pack.

---

## 📊 Step 3: The Dashboard (Power BI)
Finally, I brought it all together in an interactive dashboard. This allows stakeholders to filter by Age, Gender, and Category to see how different groups behave.

![Dashboard Placeholder](https://github.com/100rya-py/Customer-Shopping-Behaviour-Data-Analysis/blob/main/assets/screenshot/Dashboard%20Preview.png)


**Key Visual Insights:**
* **Top Category:** Clothing is the biggest revenue driver, followed by Accessories.
* **Subscriptions:** Only **27%** of customers are subscribers, leaving a huge opportunity for growth.
* **Demographics:** The "Young Adult" group contributes the most revenue ($62k), while "Seniors" contribute the least ($55k).

---

## 💡 Business Recommendations
Based on the data, here is what I would recommend to the stakeholders:
1.  **Boost Subscriptions:** Since non-subscribers make up 73% of the base, we should offer exclusive "Subscriber-Only" benefits to convert them.
2.  **Targeted Marketing:** Marketing efforts should focus heavily on the **Young Adult** demographic and the **Clothing** category, as these are our highest revenue generators.
3.  **Loyalty Program:** We identified 3,116 "Loyal" customers. We should reward these repeat buyers to ensure they don't churn.
4.  **Discount Strategy:** Products like Hats and Sneakers have a high discount usage rate (approx 50%). We need to review if these discounts are eroding our margins or driving necessary volume.
