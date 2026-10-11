# 📊 Retail Sales Analysis

Exploratory Data Analysis (EDA) of the Sample Superstore dataset using Python, Pandas, and Matplotlib to uncover sales trends, profitability patterns, and actionable business insights.

---

## 📌 Project Overview

This project analyzes retail sales data to understand how products, regions, and discounts affect sales and profit. The analysis covers 9,994 orders (rows) across 21 columns and ends with practical recommendations for improving profitability.

**Headline result:** Revenue growth alone does not drive profit. Heavy discounting and the Furniture category are the biggest drags on profitability.

---

## 🎯 Objectives

- Analyze overall sales and profit.
- Compare sales and profit across product categories.
- Identify regional sales patterns.
- Analyze monthly sales and profit trends.
- Study the relationship between sales and profit.
- Examine how discounts relate to profitability.
- Calculate profit margins.

---

## 🛠️ Tools & Technologies

| Tool | Purpose |
| --- | --- |
| Python | Core programming language |
| Pandas | Data loading, cleaning, grouping, aggregation |
| Matplotlib | Data visualization (scatter plots, trends) |
| Google Colab | Development environment |

---

## 📂 Dataset

The project uses the **Sample Superstore** dataset (`Sample - Superstore.csv`), which contains information about orders, products, sales, quantity, profit, discounts, regions, and customer segments.

**Key columns used:** Order Date, Category, Sub-Category, Region, Product Name, Sales, Profit, Quantity, Discount, Segment.

> **Note:** The file must be loaded with `encoding="latin-1"` to avoid a Unicode decoding error.

---

## 🔍 Key Findings

### Overall metrics

| Metric | Result |
| --- | --- |
| Total Sales | $2,297,200.86 |
| Total Profit | $286,397.02 |
| Overall Profit Margin | 12.47% |
| Total Quantity Sold | 37,873 |
| Unique Orders | 5,009 |
| Sales–Profit Correlation | 0.479 (moderate positive) |

### Category performance

| Category | Sales | Profit | Profit Margin |
| --- | --- | --- | --- |
| Furniture | $741,999.80 | $18,451.27 | 2.5% |
| Office Supplies | $719,047.03 | $122,490.80 | 17.0% |
| Technology | $836,154.03 | $145,454.95 | 17.4% |

### Highlights

- **Technology** generated the highest sales and profit among the three main categories.
- **Furniture** earned very little profit relative to its sales (about 2.5% margin), so its pricing, costs, and discounting need investigation.
- The **West** region had the highest sales; the **South** had the lowest.
- **November** had the highest sales in the month-of-year analysis; **February** had the lowest.
- **High discounts** (roughly 0.5 to 0.8) were frequently associated with negative profit.
- Sales and profit showed a **moderate positive correlation (0.479)**, so high sales do not guarantee high profit.

> **Caveat:** The discount–profit relationship is an observed association, not proof of causation. Category, product, and order size may also play a role.

---

## 📈 Analysis Performed

- Overall Sales and Profit Analysis
- Category-wise Analysis
- Region-wise Analysis
- Sub-category Profit Analysis (Copiers highest profit, Envelopes lowest)
- Monthly Sales and Profit Analysis
- Sales vs Profit Visualization
- Discount vs Profit Visualization
- Profit Margin Calculation

---

## 💡 Business Recommendations

1. **Review high-discount transactions** and set discount limits where profit turns negative.
2. **Investigate Furniture's low profitability** by reviewing pricing, costs, and discounts.
3. **Monitor profit margins** alongside total sales for regions, categories, and products.
4. **Analyze monthly trends** using a Year-Month timeline to support business planning.
5. **Identify products with high sales but low profit** and consider pricing or promotion changes.

---

## ▶️ How to Run

1. Clone this repository:
```bash
   git clone https://github.com/patidarparagi286-svg/retail-sales-analysis.git
   cd retail-sales-analysis
```
2. Install the required libraries:
```bash
   pip install pandas matplotlib
```
3. Place `Sample - Superstore.csv` in the project folder.
4. Open the notebook in Google Colab or Jupyter and run all cells.

**Example: loading the data**

```python
import pandas as pd

df = pd.read_csv("Sample - Superstore.csv", encoding="latin-1")
print(df.groupby("Category")[["Sales", "Profit"]].sum())
```

---

## 📚 What I Learned

- Loading, cleaning, grouping, and aggregating data with Pandas.
- Performing Exploratory Data Analysis (EDA) from shape and summaries to scatter plots.
- Visualizing relationships with Matplotlib.
- Why profit margin should be calculated as total profit ÷ total sales per category, not as an average of row-level percentages.
- Why grouping by month number mixes years, and why a Year-Month field is needed for true trends.
- Interpreting business data without confusing correlation with causation.

---

## 🚀 Future Improvements

- Data-quality checks and outlier validation.
- Segment and shipping-mode analysis.
- Top-10 product ranking by sales and profit.
- Year-Month trend charts across years.
- Interactive dashboard in Power BI or Tableau.

---

## 📄 Full Report

[Read the full project report](Retail_Sales_Analysis_Report_final.docx)

---

## 👩‍💻 Author

**Paragi Patidar**

[GitHub](https://github.com/patidarparagi286-svg) 
