# 🛒 Market Basket Analysis & Product Association Intelligence

> An end-to-end Data Science portfolio project that implements **Market Basket Analysis (MBA)** using the Apriori algorithm to uncover customer purchasing patterns, optimize retail strategies, and drive data-driven business decisions.

---

## 📊 Live Dashboard Preview
Explore the interactive Looker Studio dashboard built for this project:
👉 **[View Looker Studio Dashboard](https://datastudio.google.com/reporting/4294e830-608e-4ed3-ba07-d7e1a1ba7b14)**

---

## 🎯 Project Objective
This project is designed to analyze customer purchasing behavior through transaction data. The primary goals are to transform raw transactional data into actionable business insights and strategic recommendations, including:
* **Cross-Selling:** Recommending relevant products at checkout or in the shopping cart.
* **Product Bundling:** Grouping high-affinity products together for special promotional packages.
* **Product Placement:** Strategically positioning items to increase Average Order Value (AOV).

---

## 🛠️ Tech Stack & Libraries
* **Programming Language:** Python
* **Environment:** Google Colab, Visual Studio Code
* **Data Manipulation & Cleansing:** Pandas, NumPy, SciPy (Z-score outlier removal)
* **Machine Learning / Association Mining:** `mlxtend` (Apriori Algorithm, Association Rules)
* **Data Visualization & BI:** Google Looker Studio, Matplotlib

---

## 📈 Key Metrics Explained
Market Basket Analysis evaluates association rules using three core metrics:
1. **Support:** Measures how frequently a product or a combination of products appears across all transactions.
2. **Confidence:** Measures the likelihood that product B is purchased given that product A has already been purchased.
3. **Lift:** Measures whether the purchase of products A and B occurs more frequently than expected by random chance. A **Lift > 1** indicates a positive correlation.

---

## 📂 Project Structure
- assets/ (Dashboard screenshots and visual assets)
- market_basket_rules.csv (Processed association rules dataset for Business Intelligence)
- Market_Basket_Analysis.ipynb (Main Google Colab notebook containing end-to-end code)
- README.md (Project documentation)

---

## 🚀 Key Steps & Methodology
1. **Data Loading & Preprocessing:** Imported transactional data, handled missing values, standardized product names to lowercase, filtered out cancelled orders, and removed outliers using Z-score.
2. **Basket Transformation:** Created a sparse basket matrix and filtered transactions containing more than 1 unique product.
3. **Frequent Itemsets Mining:** Applied the Apriori algorithm with a minimum support threshold (`0.01`).
4. **Association Rules Generation:** Generated association rules using the confidence metric (`0.7`).
5. **Business Intelligence Integration:** Exported final association rules into Google Looker Studio to build an interactive dashboard.

---

## 💡 Business Insights & Strategic Recommendations
* **High-Lift Item Bundling:** Packaging high-Lift products together with special discounts to drive sales volume.
* **Smart Cross-Selling:** Deploying automated real-time *"Customers who bought this also bought..."* prompts in e-commerce.
* **Inventory Planning:** Monitoring high-Support products to ensure best-selling stock availability and minimize stockouts.

---
## 👤 Author
* **Elieser Pasaribu** — Data Analyst / Data Scientist / Machine Learning
