*** 🛍️ Customer Shopping Behavior Analysis

A complete end-to-end analytics project uncovering insights from 3,900+ customer transactions using Python, MySQL, and Power BI.

---

*** 📌 Project Overview

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

37 missing values in review_rating → handled using median per category

🧹 Exploratory Data Analysis (Python)
✔️ Data Preparation

Loaded dataset using Pandas

Summarized structure with df.info() and df.describe()

✔️ Missing Value Treatment

Imputed missing review_rating using category-wise median

✔️ Feature Engineering

Created age_group (binned ages)

Created purchase_frequency_days

Converted all column names to snake_case

Dropped redundant column promo_code_used after consistency check

✔️ Database Integration

Exported cleaned dataset to PostgreSQL for SQL analysis

🧮 SQL Analysis (PostgreSQL)
1️⃣ Revenue by Gender
Gender	Revenue
Female	$75,191
Male	$157,890
2️⃣ High-Spending Discount Users

Identified 839 customers who used a discount but still spent above the average amount.

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

Top categories where >47% purchases involve discounts:

Hat

Sneakers

Coat

Sweater

Pants

7️⃣ Customer Segmentation

Loyal Customers: 3,116

Returning Customers: 701

New Customers: 83

8️⃣ Top 3 Products per Category

Accessories: Jewelry, Sunglasses, Belt

Clothing: Blouse, Pants, Shirt

Footwear: Sandals, Shoes, Sneakers

Outerwear: Jacket, Coat

9️⃣ Repeat Buyers & Subscription

Customers with more than 5 purchases:

No subscription: 2,518

Subscribed: 958

🔟 Revenue by Age Group

Visualized using Power BI dashboard

📊 Power BI Dashboard

Interactive dashboard includes:

Revenue trends

Age-group contribution

Product popularity

Subscription impact

Shipping type comparison

Customer segmentation

📈 Business Recommendations

✔️ Boost Subscriptions through exclusive benefits
✔️ Strengthen Loyalty Programs for repeat customers
✔️ Review Discount Strategy to protect margins
✔️ Improve Product Positioning for top-rated items
✔️ Target High-Revenue Age Groups with focused marketing

🛠️ Tech Stack

Python (Pandas, NumPy)

PostgreSQL

Power BI

Jupyter Notebook

If you want, I can also add:

✅ Project folder structure
✅ Badges (Python version, SQL, Power BI, Dataset Size)
✅ Code snippets for EDA and SQL
✅ Project banner for GitHub
