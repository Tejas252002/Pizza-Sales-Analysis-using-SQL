
# 🍕 Pizza Sales Analysis using SQL

## 📌 Project Description

This project explores a real-world pizza sales dataset to uncover business insights using **MySQL**. Through structured querying and relational joins, we analyze sales performance, customer behavior, and revenue breakdowns.

---

## 🧰 Tech Stack

- **SQL (MySQL Workbench)** – Data querying and analysis  
- **CSV Files** – Used as raw data inputs  
- **DB Schema Design** – Tables created using SQL  
- **Screenshots** – Output captured for visualization

---

## 📂 Dataset Overview

The data consists of the following files:

| File | Description |
|------|-------------|
| `orders.csv` | Contains order ID, date, and time |
| `order_details.csv` | Maps orders to pizzas and quantity |
| `pizzas.csv` | Contains pizza ID, size, type ID, and price |
| `pizza_types.csv` | Maps pizza types to names and categories |

---

## 🧾 ER Diagram (Simplified)

```
orders(order_id, order_date, order_time)
   ⬇
order_details(order_details_id, order_id, pizza_id, quantity)
   ⬇
pizzas(pizza_id, size, price, pizza_type_id)
   ⬇
pizza_types(pizza_type_id, name, category)
```

---

## 📊 Business Questions Answered

### 🔹 Basic

1. **Total Orders:** `21,350`
2. **Total Revenue:** `$81,760.05`
3. **Highest Priced Pizza:** `The Greek Pizza – $35.95`
4. **Most Common Pizza Size:** `Large (L)`
5. **Top 5 Ordered Pizza Types by Quantity** (To be confirmed from remaining screenshots)

### 🔸 Intermediate

- Quantity of pizzas ordered per category  
- Orders distribution by hour of the day  
- Category-wise pizza distribution  
- Daily average number of pizzas ordered  
- Top 3 pizza types by revenue  

### 🔺 Advanced

- Percentage revenue contribution by pizza type  
- Cumulative revenue trend over time  
- Category-wise top 3 pizzas by revenue  

---

## 📌 Sample SQL Queries

```sql
-- Total Orders
SELECT COUNT(order_id) AS total_orders FROM orders;

-- Total Revenue
SELECT ROUND(SUM(od.quantity * p.price), 2) AS total_sales
FROM order_details od
JOIN pizzas p ON od.pizza_id = p.pizza_id;
```

---

## 📸 Output Screenshots

All SQL queries and their outputs are included in the `/screenshots` folder for reference.

---

## 📁 Project Structure

```
Pizza-Sales-Analysis/
├── data/
│   ├── orders.csv
│   ├── order_details.csv
│   ├── pizzas.csv
│   └── pizza_types.csv
├── screenshots/
│   └── 1.png to 11.png
├── Questions.txt
└── README.md
```

---

## 🚀 How to Use

1. Import CSV files into a MySQL database.
2. Run table creation SQL script (from screenshots).
3. Execute queries based on `Questions.txt`.
4. View insights from result grid or export to Excel/Tableau for visualization.

---

## 📬 Contact

Built by **Tejas Ubale**  
📧 Feel free to connect via [LinkedIn](#) or drop a message for collaboration.

---
