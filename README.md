# Sdq
Data Analytics Portfolio
# 🛒 Walmart Sales Analysis Dashboard – Power BI Project

## 📊 Project Overview
This project presents an interactive **Walmart Sales Dashboard** built in **Power BI**, supported by data cleaning and preparation in **Excel**.  
The dashboard reveals business performance metrics such as total revenue, sales trends, customer demographics, and departmental contributions.

> 🎯 **Goal:** Transform raw Walmart sales data into insightful and visually compelling analytics for smarter business decisions.

---

## 🧩 Dataset Description
The dataset consists of five related tables that together represent Walmart’s sales operations:

| Table | Description |
|--------|--------------|
| **Customer** | Contains customer details (name, gender, state, town) |
| **Sale** | Includes sales transactions (quantity, payment method, date, reference ID) |
| **Product** | Lists products, prices, and department IDs |
| **Employee** | Employee details and department assignments |
| **Department** | Department names and unique IDs |

---

## 🧮 Tools & Technologies
- **Microsoft Excel** → Data cleaning, missing value handling, and transformation  
- **Power BI** → Data modeling, DAX calculations, and dashboard design  
- **GitHub Pages** → Hosting portfolio projects  

---

## 🧠 Key Skills Demonstrated
✅ Data cleaning and preparation in Excel  
✅ Building relationships between multiple tables in Power BI  
✅ DAX measures for business KPIs (`SUMX`, `RELATED`, `DISTINCTCOUNT`)  
✅ Handling missing data with clarity and transparency  
✅ Designing interactive dashboards for business storytelling  

---

## 📈 Dashboard Insights
- Total sales reached **$15.75M**, with top-performing departments including **Sports & Outdoors** and **Clothing**.  
- **Cash and debit cards** were the most popular payment methods.  
- Sales showed fluctuations across years, with visible recovery trends in 2024.  
- Gender distribution remained balanced, showing consistent customer engagement.   
---

## 🧾 Dashboard Preview

### 💻 Power BI Dashboard
![Dashboard Preview](images/dashboard_preview.png)

## 🧰 DAX Measures Used

```DAX
Total Sales = SUMX(Sale, Sale[quantity] * RELATED(Product[price]))
Total Quantity = SUM(Sale[quantity])
Unique Customers = DISTINCTCOUNT(Sale[customer_id])
Average Sales per Customer = DIVIDE([Total Sales], [Unique Customers])
