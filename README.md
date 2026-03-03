# 🏠 Toronto Airbnb Market Analysis — SQL Project

**Tool Used:** SQLite (DB Browser for SQLite)  
**Dataset:** Inside Airbnb — Toronto Listings  
**Source:** [insideairbnb.com/toronto](http://insideairbnb.com/toronto/)  
**Total Listings Analyzed:** 21,468

---

## 📌 Project Overview

This project analyzes Toronto's Airbnb market using SQL to uncover pricing trends, host behaviour, neighbourhood popularity, and availability patterns. All analysis was performed using raw CSV data imported into SQLite.

---

## 🔍 Key Findings

- **Waterfront Communities dominates** Toronto Airbnb with 3,542 listings — 4x more than the second-ranked neighbourhood (Niagara, 834)
- **Scarborough Village is the most expensive** neighbourhood at $657/night average — surprisingly beating wealthy areas like Bridle Path ($650)
- **66% of listings are entire homes** — Airbnb in Toronto competes with the rental housing market, not hotels
- **Wendy has 121 listings alone** — Toronto Airbnb is largely run by commercial operators, not casual home sharers
- **6,716 listings available almost year-round** — confirming the commercial nature of the platform
- **4,445 ghost listings** exist (20% of all listings) — hosts who listed but are no longer active
- **Weekly stays dominate at 58%** of all listings — Toronto attracts longer-term remote workers and travelers
- **Data quality issue discovered:** price column stored as TEXT not INTEGER — fixed using CAST()

---

## 📊 Queries Included

| # | Query | Insight |
|---|---|---|
| 1 | Listings by Neighbourhood | Waterfront leads with 3,542 listings |
| 2 | Average Price by Neighbourhood | Scarborough Village most expensive at $657/night |
| 3 | Room Type Breakdown with % | 66% entire homes, only 0.08% hotel rooms |
| 4 | Top Hosts by Listing Count | Wendy has 121 listings — commercial operator |
| 5 | Price Analysis by Room Type | Entire homes 3x more expensive than private rooms |
| 6 | Most Reviewed Neighbourhoods | Kingsview Village highest avg reviews (73.92) |
| 7 | Stay Category Analysis | 58% of listings require weekly minimum stay |
| 8 | Availability Analysis | 6,716 listings available 271–365 days/year |
| 9 | Price Outliers & Data Quality | Discovered TEXT vs INTEGER data type bug |
| 10 | Final Master Summary | Combined neighbourhood overview with CAST fix |

---

## 🛠️ SQL Concepts Used

- `SELECT`, `FROM`, `WHERE`, `GROUP BY`, `ORDER BY`
- Aggregate functions: `COUNT()`, `AVG()`, `SUM()`, `MIN()`, `MAX()`, `ROUND()`
- `CASE WHEN / THEN / ELSE / END` — conditional logic
- `BETWEEN` — range filtering
- Subqueries — query inside a query
- `CAST()` — data type conversion
- `LIMIT` — result limiting
- Percentage calculations using subqueries

---

## 📁 Project Structure

```
airbnb-toronto-sql-analysis/
│
├── README.md
├── listings.csv                         # Raw dataset from Inside Airbnb
│
└── screenshots/
    ├── 01_neighbourhood_listings.png
    ├── 02_avg_price_neighbourhood.png
    ├── 03_room_type_breakdown.png
    ├── 04_top_hosts.png
    ├── 05_price_by_room_type.png
    ├── 06_most_reviewed_neighbourhoods.png
    ├── 07_stay_categories.png
    ├── 08_availability_analysis.png
    ├── 09_price_outliers.png
    └── 10_final_summary.png
```

---

## 👩‍💻 About

**Rubisha Jyakhwo**  
Aspiring Data Analyst | HackerRank SQL Advanced Certified  
📍 Toronto, Canada  
🔗 [LinkedIn Profile](#) 

---

*This is Project 1 of my data analytics portfolio. Built entirely from scratch with real Toronto data.*
