# 🛍️ **Customer Shopping Behavior Analysis**

A complete end-to-end analytics project uncovering insights from **3,900+ customer transactions** using **Python**, **MySQL**, and **Power BI**.

---

## 📌 **Project Overview**
This project analyzes customer shopping behavior to uncover:

- **Spending patterns**  
- **Product preferences**  
- **Customer segmentation**  
- **Subscription impacts**  

These insights help businesses refine **marketing strategy**, **pricing**, **inventory decisions**, and **customer retention programs**.

---

## 📂 **Dataset Summary**
- **Rows:** 3,900  
- **Columns:** 18  

### **Data Includes**
- **Demographics:** Age, Gender, Location, Subscription  
- **Purchase Details:** Item, Category, Amount, Season, Size, Color  
- **Behavior:** Discount usage, Promo Code, Review Rating, Previous Purchases, Shipping Type  

### **Missing Data**
- 37 missing values in `review_rating` → handled using **category-wise median**

---

## 🧹 **Exploratory Data Analysis (Python)**

### ✔️ **Data Preparation**
- Loaded dataset using **Pandas**
- Used `df.info()` and `df.describe()` for structure & statistical summary

### ✔️ **Missing Value Handling**
- Imputed missing **review_rating** using **median per product category**

### ✔️ **Feature Engineering**
- Created **age_group** by binning age  
- Created **purchase_frequency_days**  
- Converted all column names to **snake_case**  
- Removed redundant `promo_code_used` column  

### ✔️ **Database Integration**
- Loaded cleaned DataFrame into **PostgreSQL** for deeper SQL-based analysis  

---

## 🧮 **SQL Analysis (PostgreSQL)**

### **1️⃣ Revenue by Gender**
| **Gender** | **Revenue** |
|-----------|-------------|
| Female    | **$75,191** |
| Male      | **$157,890** |

---

### **2️⃣ High-Spending Discount Users**
- **839 customers** used discounts but still spent **more than the average purchase amount**.

---

### **3️⃣ Top 5 Highest-Rated Products**
1. **Gloves — 3.86**  
2. **Sandals — 3.84**  
3. **Boots — 3.82**  
4. **Hat — 3.80**  
5. **Skirt — 3.78**

---

### **4️⃣ Shipping Type Comparison**
| **Shipping Type** | **Avg Spend** |
|-------------------|---------------|
| Standard          | **$58.46**    |
| Express           | **$60.48**    |

---

### **5️⃣ Subscription Insights**
| **Subscription** | **Customers** | **Avg Spend** | **Total Revenue** |
|------------------|----------------|----------------|-------------------|
| Yes              | 1053           | 59.49          | 62,645            |
| No               | 2847           | 59.87          | 170,436           |

📌 **Non-subscribers generate higher total revenue.**

---

### **6️⃣ Discount-Dependent Products**
Products where **47%+ customers use discounts**:
- **Hat**
- **Sneakers**
- **Coat**
- **Sweater**
- **Pants**

---

### **7️⃣ Customer Segmentation**
- **Loyal Customers:** 3,116  
- **Returning Customers:** 701  
- **New Customers:** 83  

---

### **8️⃣ Top 3 Products by Category**
- **Accessories:** Jewelry, Sunglasses, Belt  
- **Clothing:** Blouse, Pants, Shirt  
- **Footwear:** Sandals, Shoes, Sneakers  
- **Outerwear:** Jacket, Coat  

---

### **9️⃣ Repeat Buyers & Subscription**
Customers with **more than 5 purchases**:
- **Non-subscribers:** 2,518  
- **Subscribers:** 958

---

### **🔟 Revenue by Age Group**
- Visualized using **Power BI dashboard**

---

## 📊 **Power BI Dashboard**
The dashboard includes interactive visuals for:

- Revenue trends  
- Age-group performance  
- Product category insights  
- Subscription impact  
- Shipping type comparison  
- Customer segmentation  

---

## 📈 **Business Recommendations**
✔️ **Promote subscriptions** through exclusive benefits  
✔️ **Strengthen loyalty programs** for returning customers  
✔️ **Optimize discount policies** to avoid margin losses  
✔️ **Highlight best-performing products** in campaigns  
✔️ **Target high-revenue age groups** with focused marketing  

---

## 🛠️ **Tech Stack**
- **Python:** Pandas, NumPy  
- **SQL:** PostgreSQL  
- **Visualization:** Power BI  
- **Notebook:** Jupyter Notebook  

---

## 🚀 **How to Use**
1. Clone the repository:
   ```bash
   git clone https://github.com/YourUsername/Customer-Shopping-Behavior-Analysis.git

---

# ***👨‍💻 Author***

**Md Shah Alam**  
Data Analyst | SQL • Python • Power BI • Excel  

📧 Email: **mdshahalam906565@gmail.com**  

🔗 GitHub: **https://github.com/MdShahAlamDA**  

🔗 LinkedIn: **https://www.linkedin.com/in/md-shah-alam-671602343/**  

*Passionate about turning raw data into meaningful insights and business value.*

---

⭐ **If you found this project helpful, don’t forget to give it a star on GitHub!**

