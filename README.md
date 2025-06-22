
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

## 📊 Insights & Metrics

- **Total Orders:** `21,350`
- **Total Revenue:** `$81,760.05`
- **Highest Priced Pizza:** `The Greek Pizza – $35.95`
- **Most Common Pizza Size Ordered:** `Large (L)`
- **Pizza Category by Quantity:**
  - Classic: 14,888  
  - Supreme: 11,987  
  - Veggie: 11,649  
  - Chicken: 11,050
- **Orders by Hour (Peak Time):**
  - Most orders between 12:00 PM – 8:00 PM, with peak at 1:00 PM and 6:00–7:00 PM.
- **Category-wise Pizza Count:**
  - Chicken: 6 types  
  - Classic: 8 types  
  - Supreme: 9 types  
  - Veggie: 9 types
- **Average Pizzas Ordered Per Day:** `138`

---

## 📸 Output Screenshots

All SQL queries and their outputs are included in the `/screenshots` folder. These include:
- Table creation queries
- Revenue and order calculations
- Grouping and aggregations
- Category-based analysis
- Time-based ordering behavior

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
│   └── 1.png to 10.png
├── Questions.txt
└── README.md
```

---

## 🚀 How to Use

1. Import CSV files into a MySQL database.
2. Run table creation SQL script (refer to `1.png`).
3. Execute the SQL queries as shown in the screenshots.
4. Analyze the outputs and derive insights or visualize in BI tools.

---

## 📬 Contact

Built by **Tejas Ubale**  
📧 Feel free to connect via [LinkedIn](#) or drop a message for collaboration.

---
