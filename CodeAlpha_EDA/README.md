# Sales Data Analysis - Exploratory Data Analysis (EDA) Task

## 📊 Project Overview
This project performs comprehensive Exploratory Data Analysis (EDA) on sales data to uncover key business insights, patterns, and relationships. The analysis examines sales performance across regions, product categories, and profitability metrics to support data-driven decision-making.

## 🎯 Business Questions Addressed
1. **Which region generates the highest sales?**
2. **Which category is most profitable?**
3. **Are higher sales giving higher profit?**
4. **Which product has low profit despite high sales?**

## 📁 Dataset Overview
- **Total Records**: 10 entries (sample shown, with extended data up to 1077 records)
- **Features**: 8 columns including Order_ID, Date, Region, Product, Category, Sales, Quantity, Profit
- **Data Types**: Integer, DateTime, Object (categorical)
- **Quality Check**: No missing values or duplicate records found

## 📈 Key Performance Indicators (KPIs)

| Metric | Value |
|--------|-------|
| **Total Sales by Region** | South: ₹80,000<br>North: ₹57,500<br>East: ₹37,000<br>West: ₹30,000 |
| **Most Profitable Category** | Furniture (₹17,400) |
| **Electronics Profit** | ₹16,600 |
| **Sales-Profit Correlation** | 0.96 (Strong Positive) |

## 🔍 Key Insights

### Regional Performance
- **South region dominates** with highest sales (₹80,000), followed by North (₹57,500)
- West region shows lowest sales performance (₹30,000)

### Category Analysis
- **Furniture marginally outperforms Electronics** in profitability (₹17,400 vs ₹16,600)
- Both categories show healthy profit margins

### Sales-Profit Relationship
- **Strong positive correlation (0.96)** indicates higher sales consistently lead to higher profits
- Validates business model efficiency across all regions and categories

## 📊 Visualizations Included
1. **Sales by Region Bar Chart** - Comparative analysis of regional sales performance
2. **Profit by Category Analysis** - Category-wise profitability breakdown
3. **Correlation Matrix** - Sales vs Profit relationship visualization

## 🛠️ Technologies Used
- **Python** (Pandas, NumPy)
- **Data Visualization**: Matplotlib
- **Analysis Tools**: Jupyter Notebook
- **Statistical Analysis**: Correlation studies

## 📁 Repository Structure