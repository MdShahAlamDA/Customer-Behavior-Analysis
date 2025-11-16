🛍️ Customer Shopping Behavior Analysis

A complete end-to-end analytics project uncovering insights from 3,900+ customer transactions using Python, PostgreSQL, and Power BI.

📌 Project Overview

This project analyzes customer shopping patterns to understand:

Spending behavior

Product preferences

Customer segmentation

Subscription trends

The insights help businesses optimize marketing strategy, pricing, product positioning, and customer retention.

📂 Dataset Summary

Rows: 3,900

Columns: 18

Data Fields Include

Demographics: Age, Gender, Location, Subscription status

Purchase Details: Item, Category, Amount, Season, Size, Color

Behavior: Discount usage, Promo Code, Previous Purchases, Review Rating, Shipping Type

Missing Values

37 missing values in review_rating → imputed using median per category

🧹 Exploratory Data Analysis (Python)
✔️ Data Preparation

Loaded dataset using Pandas

Used df.info() and df.describe() for structural & statistical summary

✔️ Missing Value Treatment

Imputed missing review_rating values using category-wise median

✔️ Feature Engineering

Created age_group (binned ages)

Derived purchase_frequency_days

Standardized columns to snake_case

Dropped redundant promo_code_used column after correlation check

✔️ Database Integration

Loaded cleaned data into PostgreSQL for SQL analysis

🧮 SQL Analysis (PostgreSQL)
1️⃣ Revenue by Gender
Gender	Revenue
Female	$75,191
Male	$157,890
2️⃣ High-Spending Discount Users

Identified 839 customers who used a discount but still spent above average.

3️⃣ Top 5 Products by Review Rating

Gloves — 3.86

Sandals — 3.84

Boots — 3.82

Hat — 3.80

Skirt — 3.78

4️⃣ Shipping Type Comparison
Shipping Type	Avg Spend
Standard	$58.46
Express	$60.48
5️⃣ Subscription Insights
Subscription	Customers	Avg Spend	Total Revenue
Yes	1053	59.49	62,645
No	2847	59.87	170,436

📌 Non-subscribers generate more total revenue.

6️⃣ Discount-Dependent Products

More than 47% of purchases include discounts for:

Hat

Sneakers

Coat

Sweater

Pants

7️⃣ Customer Segmentation

Loyal Customers: 3,116

Returning Customers: 701

New Customers: 83

8️⃣ Top 3 Products Per Category

Accessories: Jewelry, Sunglasses, Belt

Clothing: Blouse, Pants, Shirt

Footwear: Sandals, Shoes, Sneakers

Outerwear: Jacket, Coat

9️⃣ Repeat Buyers vs Subscription

Customers with >5 purchases:

No subscription: 2,518

Subscription: 958

🔟 Revenue by Age Group

Visualized using Power BI.

📊 Power BI Dashboard

An interactive dashboard visualizing:

Revenue trends

Age-group distribution

Product popularity

Subscription impact

Shipping type analysis

Customer segmentation

📈 Business Recommendations

✔️ Promote subscriptions with exclusive benefits
✔️ Strengthen loyalty programs to convert returning → loyal customers
✔️ Review discount policy to protect margins
✔️ Highlight top-rated and best-selling items
✔️ Target high-revenue age groups with focused marketing

🛠️ Tech Stack

Python (Pandas, NumPy)

PostgreSQL

Power BI

Jupyter Notebook

If you want, I can also add:
✅ Project banner
✅ Folder structure
✅ Badges (Python version, PostgreSQL, Power BI, Dataset size)
✅ Code samples for SQL & EDA
