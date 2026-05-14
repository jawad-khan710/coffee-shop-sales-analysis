# ☕ Coffee Shop Sales Analysis

> **End-to-end Exploratory Data Analysis (EDA) of real coffee shop transactions — uncovering revenue drivers, peak hours, top products, and profit trends using Python.**

---

## 📌 Project Overview

This project performs a complete data analysis pipeline on a coffee shop's transactional sales dataset. The goal is to extract actionable business insights that can guide product strategy, inventory planning, and revenue growth.

**Analyst:** Jawad Khan — Aspiring Data Analyst

---

## 🎯 Business Questions Answered

| # | Question |
|---|----------|
| 1 | Which products generate the most revenue and profit? |
| 2 | What are the busiest hours, days, and months? |
| 3 | Which product sizes (Small / Regular / Large) sell the most? |
| 4 | What percentage of total profit comes from the top 5 products? |
| 5 | Are there any products running at a loss? |
| 6 | Can we predict profit using transaction features? |

---

## 📂 Project Structure

```
coffee-shop-sales-analysis/
│
├── Coffee_Shop_Sales.xlsx           # Raw dataset (149,116 transactions)
├── Coffee_Shop_Sales_Analysis.ipynb # Main analysis notebook
├── requirements.txt                 # Python dependencies
└── README.md                        # Project documentation
```

---

## 🗃️ Dataset

The dataset contains **149,116 sales transactions** from **3 store locations** in New York City:

| Column | Description |
|--------|-------------|
| `transaction_id` | Unique transaction identifier |
| `transaction_date` | Date of the transaction |
| `transaction_time` | Time of the transaction |
| `transaction_qty` | Number of items purchased |
| `store_id` | Store identifier |
| `store_location` | Store name (Lower Manhattan, Hell's Kitchen, Astoria) |
| `product_id` | Product identifier |
| `unit_price` | Selling price per unit |
| `product_category` | Category (Coffee, Tea, Bakery, etc.) |
| `product_type` | Type within the category |
| `product_detail` | Full product name with size |

---

## 🔧 Tech Stack

![Python](https://img.shields.io/badge/Python-3.10+-blue?logo=python)
![Pandas](https://img.shields.io/badge/Pandas-2.0-lightblue?logo=pandas)
![NumPy](https://img.shields.io/badge/NumPy-1.26-orange?logo=numpy)
![Matplotlib](https://img.shields.io/badge/Matplotlib-3.8-blueviolet)
![Seaborn](https://img.shields.io/badge/Seaborn-0.13-teal)
![Scikit-learn](https://img.shields.io/badge/Scikit--Learn-1.4-red?logo=scikit-learn)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange?logo=jupyter)

---

## 📊 Analysis Workflow

```
1. Import Libraries
      ↓
2. Load Dataset
      ↓
3. Data Cleaning
   • No null values found
   • No duplicate rows found
      ↓
4. Feature Engineering
   • Revenue = transaction_qty × unit_price
   • Extracted: hour, day, month from datetime
   • Extracted: product size (Sm/Rg/Lg → Small/Regular/Large)
   • Estimated cost_per_unit and profit_loss
      ↓
5. Exploratory Data Analysis (EDA)
   • Product-level sales & revenue breakdown
   • Hourly, daily, monthly transaction trends
   • Store-location performance comparison
   • Size preference analysis
      ↓
6. Predictive Modeling
   • Linear Regression to predict profit
   • Features: qty, store_id, unit_price, cost_per_unit
      ↓
7. Business Insights & Recommendations
```

---

## 💡 Key Findings

- **Top 5 products generate 31% of total profit** — high concentration worth protecting.
- **Regular size** is the most purchased across all product categories.
- **Peak hours** fall mid-morning, aligned with typical commuter coffee runs.
- **Brazilian, Our Time Diner Blend, Columbian Medium Roast, Ethiopia,** and **Jamaican Coffee River** are the best-selling products.
- All major products generated positive profit — no significant loss-making items found.

---

## 📈 Business Recommendations

1. **Prioritize top 5 products** in marketing campaigns and loyalty programs.
2. **Stock more Regular-size items** — they outsell Small by a large margin.
3. **Staff up during peak morning hours** to reduce wait times and capture more sales.
4. **Bundle slow-moving products** with best-sellers to boost their visibility.
5. **Collect more granular customer data** to enable segmentation in the future.

---

## 🚀 Future Improvements

- [ ] Time-series forecasting for monthly sales
- [ ] Customer segmentation using clustering
- [ ] Interactive dashboard (Power BI / Tableau)
- [ ] ML-based product recommendation system
- [ ] Anomaly detection for unusual transactions

---

## ⚙️ How to Run

```bash
# 1. Clone the repository
git clone https://github.com/jawad-khan710/coffee-shop-sales-analysis.git
cd coffee-shop-sales-analysis

# 2. Install dependencies
pip install -r requirements.txt

# 3. Launch the notebook
jupyter notebook Coffee_Shop_Sales_Analysis.ipynb
```

---

## 📬 Connect with Me

> *This project was built as part of my Data Analytics learning journey.*
> LinkedIn:(www.linkedin.com/in/jawad-khan-133755408)

