
# 🍕 Pizza Sales Analysis using SQL

## 📌 Project Description

This project explores a real-world pizza sales dataset to uncover business insights using **MySQL**. Through structured querying and relational joins, we analyze sales performance, customer behavior, and revenue breakdowns.

---

## 🧰 Tech Stack

- **SQL (MySQL Workbench)** – Data querying and analysis  
- **CSV Files** – Used as raw data inputs  
- **ER Model + Queries** – To extract actionable metrics  
- **Screenshots** – Visual proof of SQL results

---

## 📂 Dataset Overview

| File | Description |
|------|-------------|
| `orders.csv` | Contains order ID, date, and time |
| `order_details.csv` | Maps orders to pizzas and quantity |
| `pizzas.csv` | Pizza ID, size, price, and type |
| `pizza_types.csv` | Pizza name and category |

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

## 📊 Insights & Metrics

- **Total Orders:** `21,350`
- **Total Revenue:** `$81,760.05`
- **Highest Priced Pizza:** `The Greek Pizza – $35.95`
- **Most Common Pizza Size:** `Large (L)`
- **Most Ordered Pizza Type (by quantity):** `The Classic Deluxe Pizza`
- **Average Pizzas Ordered per Day:** `138`
- **Top 3 Pizza Types by Revenue:**  
  - The Thai Chicken Pizza  
  - The Barbeque Chicken Pizza  
  - The California Chicken Pizza
- **Top 3 Revenue Pizzas per Category:** Uses `RANK()` with `PARTITION BY`
- **Category-wise % Revenue Contribution:** Classic (26.91%), Supreme (25.46%)...
- **Orders by Hour:** Peak from 12 PM – 8 PM
- **Cumulative Revenue Trend:** Steady daily growth

---

## 🖼️ Screenshot Highlights

### 📌 1. Table Creation  
`orders` and `order_details` schema definition.  
![1.png](screenshots/1.png)

### 📌 2. Total Orders  
Query to count number of orders placed.  
![2.png](screenshots/2.png)

### 📌 3. Total Revenue  
Calculates revenue using joined tables.  
![3.png](screenshots/3.png)

### 📌 4. Highest Priced Pizza  
Identifies the costliest pizza.  
![4.png](screenshots/4.png)

### 📌 5. Most Ordered Size  
Shows size-wise pizza demand.  
![5.png](screenshots/5.png)

### 📌 6. Top 5 Pizza Types by Quantity  
Ranks pizza types by number of units sold.  
![6.png](screenshots/6.png)

### 📌 7. Quantity per Category  
Sums pizzas ordered by category.  
![7.png](screenshots/7.png)

### 📌 8. Orders by Hour  
Groups orders to show hourly distribution.  
![8.png](screenshots/8.png)

### 📌 9. Pizza Count per Category  
Counts how many unique pizzas exist per category.  
![9.png](screenshots/9.png)

### 📌 10. Average Pizzas per Day  
Averages total pizzas sold daily.  
![10.png](screenshots/10.png)

### 📌 11. Top 5 Pizzas by Revenue  
Lists pizzas that made the most money.  
![11.png](screenshots/11.png)

### 📌 12. Revenue % per Category  
Shows which category contributes what % to total revenue.  
![12.png](screenshots/12.png)

### 📌 13. Cumulative Revenue by Day  
Tracks sales revenue accumulating over time.  
![13.png](screenshots/13.png)

### 📌 14. Top 3 Revenue Pizzas per Category  
Uses `RANK()` + `PARTITION BY` to segment results.  
![14.png](screenshots/14.png)

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
│   ├── 1.png ... 14.png
├── Questions.txt
└── README.md
```

---

## 🚀 How to Run

1. Create the database schema in MySQL
2. Load the `.csv` files using `LOAD DATA INFILE` or import wizard
3. Execute each query from the screenshots
4. View result sets and analyze key trends

---

## 📬 Contact

Built by **Tejas Ubale**  
📧 Reach out on [LinkedIn](#)

---
