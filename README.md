# Blinkit_BI
 Power BI Blinkit sales analysis

## 📌 Overview
This Power BI project provides a 360-degree analytical view of **Blinkit**, a last-minute grocery delivery app in India. Built by following a structured video tutorial and customized further, this dashboard enables deep analysis of:
- 🏪 Outlet performance by size, type, and tier
- 🛒 Item sales, types, fat content
- ⭐ Customer satisfaction metrics
- 📍 Regional and temporal sales patterns

## 🌟 Features & KPIs
This dashboard is made with powerful KPIs and interactive visuals:

### 🎯 Key Performance Indicators (KPIs)

| KPI | Description |
|-----|-------------|
| **Total Sales** | Sum of all item sales across all outlets |
| **Average Sales per Outlet** | Total Sales ÷ Number of Outlets |
| **Number of Items** | Total distinct items sold |
| **Average Rating** | Mean customer rating of sold items |
| **Item Visibility** | Visibility percentage of each item in the dataset |
| **Sales by Year** | Line/area chart showing sales growth from 2012–2022 |
| **Sales by Outlet Tier** | Distribution across Tier 1, 2, and 3 cities |
| **Sales by Outlet Size** | Pie chart showing small, medium, and high outlet size contribution |
| **Sales by Fat Content** | Bubble/pie chart comparison of "Low Fat" and "Regular" items |
| **Top 10 Item Types** | Bar chart of most-sold items with their count, rating, and sales |
| **Outlet Type Table** | Tabular KPI summary (Sales, Items, Ratings, Visibility) per outlet type |

## 💡 Key Insights
- 📈 **Tier 3 outlets outperform others**, driving the largest revenue share.
- 🧁 **Low Fat items** show a healthier rating average, while **Regular Fat** leads in volume.
- 🛒 **Fruits and Snacks dominate** as top-selling item categories.
- 📍 **Outlet size and location** significantly affect item visibility and sales patterns.
- 🔍 **Customer ratings remain stable**, suggesting consistent product quality.

---

### 🔗 Relationships
- Built 1-to-many relationships between tables using `Item_Type` and `Outlet_Identifier`
- All KPIs use **DAX** and are filtered by slicers across **year, tier, size, and fat content**

### 🧠 Sample DAX Measures

```dax
Total Sales = SUM(Metrics[Total_Sales])
Average Sales = AVERAGE(Metrics[Total_Sales])
Item Visibility = AVERAGE(Grocery[Item_Visibility])
Average Rating = AVERAGE(Grocery[Rating])
```

🙏 Acknowledgements
📺 Power BI Blinkit Project Tutorial
This project was created by learning and extending this tutorial as a personal challenge.
