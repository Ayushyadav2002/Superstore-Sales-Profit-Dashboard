# 📊 Superstore Sales & Profit Dashboard
**Interactive Power BI dashboard uncovering key profit drivers, regional performance, and discount inefficiencies across 9,994+ retail transactions (2014–2017).**

---

## 🎯 Project Overview

**Objective:**  
Build an interactive sales analytics dashboard to help business managers identify top-performing regions, optimize product strategies, and address profitability issues.

**Tools Used:**  
Power BI Desktop · Power Query · DAX

**Dataset:**  
[Kaggle Superstore Dataset – by Vivek468](https://www.kaggle.com/datasets/vivek468/superstore-dataset-final)  
(9,994 rows · 21 columns)

---

## 📈 Dashboard Features

### **Key Performance Metrics**
- 💰 **Total Sales:** $1.10M  
- 📈 **Total Profit:** $132.52K  
- 📦 **Total Quantity Sold:** 19K units  
- 💸 **Average Discount:** 15.7%  
- 🧮 **Overall Profit Margin:** 12.05%

### **Visualizations**
1. **Sales by Region** – Horizontal bar chart highlighting regional sales distribution  
2. **Sales & Profit by Category** – Clustered column chart comparing revenue vs profit  
3. **Sales Trend Over Time** – Line chart tracking growth from 2014–2017  
4. **Profitability by Sub-Category** – Scatter plot separating profitable and loss-making products  
5. **Top 10 Products by Sales** – Table showing highest-revenue items  
6. **Interactive Filters (Slicers)** – Region, Year, and Category for easy data exploration

---

## 🔍 Key Insights

### **Regional Performance**
- **West region leads** with **$332.44K in sales (14.26% of total revenue)**  
- East and Central regions maintain stronger profit margins

### **Category Analysis**
- **Technology** category shows the **highest profit margin (18.43%)**  
- **Furniture** underperforms heavily with only **2.03% margin**

### **Loss-Making Products**
- **Tables sub-category** incurs a **$-10,997.07 loss** despite strong sales volume  
- Indicates **over-discounting** or inefficient cost control

### **Growth Over Time**
- Sales increased **12.05% between 2014–2017**  
- Strongest annual growth occurred in **2016**

---

## 💡 Business Recommendations

1. **Review Table sub-category pricing** to mitigate the $11K loss.  
2. **Scale up Technology category** — strong demand and highest profit margin.  
3. **Reduce excessive discounts** in Furniture — focus on profitability, not volume.  
4. **Leverage West region** as the benchmark for regional expansion strategies.  

---

## 🛠️ Technical Implementation

### **Data Preparation**
- Imported CSV data into Power BI  
- Cleaned dataset via Power Query (handled nulls, duplicates, corrected data types)  
- Created new columns: **Year**, **Month Name**, **Profit Margin %**

### **DAX Measures Created**
```dax
Total Sales = SUM('Sample - Superstore'[Sales])
Total Profit = SUM('Sample - Superstore'[Profit])
Total Quantity = SUM('Sample - Superstore'[Quantity])
Average Discount = AVERAGE('Sample - Superstore'[Discount])
Profit Margin % = DIVIDE([Total Profit], [Total Sales], 0)
```

### **Dashboard Design**
- Applied professional color theme for visual consistency  
- Enabled cross-filtering across all visualizations  
- Added interactive slicers for dynamic exploration

---

## 📂 Repository Contents

- `Superstore_Sales_Dashboard.pbix` – Power BI dashboard file  
- `Sample - Superstore.csv` – Source dataset  
- `Dashboard_Screenshot.png` – Dashboard preview  
- `README.md` – Project documentation

---

## 🚀 How to Use

1. Download [Power BI Desktop](https://powerbi.microsoft.com/desktop/) (free)  
2. Clone this repository or download the `.pbix` file  
3. Open `Superstore_Sales_Dashboard.pbix` in Power BI Desktop  
4. Use slicers to filter by **Region**, **Year**, or **Category**  
5. Click any chart element to cross-filter other visuals

---

## 📊 Dashboard Preview

![Superstore Dashboard](Superstore_Dashboard_Screenshot.png)

---

## 👤 Author

**Ayush Yadav**  
📧 Email: Ayushy0302@gmail.com  
💼 LinkedIn: Ayush Yadav
🐙 GitHub: Ayushyadav2002

---

## 📝 License & Dataset Source

Dataset: [Kaggle Superstore Dataset](https://www.kaggle.com/datasets/vivek468/superstore-dataset-final)  
This project is for educational and portfolio purposes.
