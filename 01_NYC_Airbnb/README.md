# 🏙️ NYC Airbnb Market Analysis (Sprint 1)

**Project Title**: Manhattan Vacation Rental Investment Insights  
**Program**: TripleTen – Business Intelligence Analyst  
**Tools Used**: Microsoft Excel (Pivot Tables, Formulas, Data Cleaning)

## 📌 Objective
Help a client make informed investment decisions by identifying:
- The most attractive neighborhoods for vacation rentals
- The most popular property sizes
- Estimated annual revenue for top-performing listings

## 🧹 Data Cleaning
Performed cleaning on the following fields:
- `neighborhood`: Standardized capitalization and removed extra spaces → `neighborhood_clean`
- `bedrooms`: Handled empty cells and categorized studios as 0 → `bedrooms_clean`

## 📊 Analysis
- Used `number_of_reviews_ltm` to identify high-demand neighborhoods (proxy for popularity)
- Created pivot tables to examine:
  - Top 10 neighborhoods for vacation rentals
  - Most popular bedroom counts across neighborhoods
- Determined that **1-bedroom units** are most popular across most top neighborhoods

## 💰 Revenue Estimation
- Used 30-day calendar data to calculate revenue per listing:
  - Created `revenue_earned` using `adjusted_price` only when listings were available
  - Aggregated revenue using `SUMIF` into the listings table
- Estimated annual revenue by multiplying 30-day totals by 12

**Top Listing ID**: `49946551`  
**Estimated Monthly Revenue**: `$29,940`  
**Estimated Annual Revenue**: `$359,280`

## ✅ Key Takeaways
- **Lower East Side, Hell's Kitchen, and Harlem** are prime areas for vacation rentals.
- **1-bedroom units** are most profitable across most neighborhoods.
- Listings that match the preferred size and location can generate **over $300K annually**.

---

> 📁 This project is part of my Business Intelligence Analyst portfolio.  
> 📫 Feel free to connect or reach out if you'd like to collaborate or learn more!
