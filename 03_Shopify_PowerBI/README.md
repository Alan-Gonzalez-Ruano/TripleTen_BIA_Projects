# 🛍️ Shopify App Store Power BI Report (Sprint 6)

**Project Title**: Analyzing App Success on Shopify  
**Program**: TripleTen – Business Intelligence Analyst  
**Tools Used**: Power BI (DAX, Relationships, Data Modeling)

---

## 📌 Objective
Explore how review counts, ratings, and developer responsiveness contribute to app success on the Shopify App Store.

---

## 📁 Data Structure
- `apps`: App details (developer, rating, review count)
- `reviews`: Customer feedback with rating, helpful count, developer reply
- `categories`, `apps_categories`: App classification tags

---

## 📈 Visualizations & DAX Logic

### 🔹 Page 1: App Landscape
- KPI Card: Total number of apps
- Line Chart: Reviews over time (`lastmod` field)
- Scatterplot: Review count vs. average rating (with interpretation)

### 🔹 Page 2: Reviews
- `helpful_reviews = rating * (1 + helpful_count)`
- `developer_answered = IF(ISBLANK(developer_reply), 0, 1)`
- Scatterplot: Developer response vs. rating

### 🔹 Page 3: Developer Insights
- Relationship: `Reviews.app_id` → `Apps.id`
- Bar Charts:
  - Developer vs. sum of ratings (misleading!)
  - Developer vs. average `helpful_reviews`
  - Developer responsiveness (filtered by >500 reviews)

---

## 🧠 Key Takeaways
- Review volume doesn’t always equal quality
- Developers who reply to feedback tend to have better average ratings
- Helpful review weighting gives deeper insight into app performance

> 📁 This project demonstrates my ability to model data, write DAX, and build interactive visuals using Power BI.
