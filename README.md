# Coffee-Shop-Sales-Analysis

## 📌 Project Overview

This project analyzes coffee shop retail sales data using **Microsoft Excel** to identify sales patterns, product performance, store performance, and customer ordering trends.

The main objective is to turn raw transaction data into an interactive dashboard that can be used to understand the business's sales performance and identify actionable insights.

## 🎯 Objectives

The analysis aims to answer the following questions:

* How do sales vary by day of the week and hour of the day?
* What are the peak times for sales activity?
* What is the total sales revenue for each month?
* How do sales vary across different store locations?
* What is the average order value?
* Which products perform best in terms of quantity and revenue?
* How do sales vary by product category and product type?


---

## 📂 Dataset

The analysis is based on the **Coffee Shop Sales** transaction dataset.

### Dataset Overview

| Metric                  |       Value |
| ----------------------- | ----------: |
| Total Transactions      |     149,116 |
| Total Quantity Sold     |     214,470 |
| Total Revenue           | €698,812.33 |
| Average Order Value     |       €4.69 |
| Average Items per Order |        1.44 |
| Average Selling Price   |       €3.26 |
| Store Locations         |           3 |
| Product Categories      |           9 |

### Main Dataset Fields

The dataset contains information about:

* Transaction ID
* Transaction Date
* Transaction Time
* Transaction Quantity
* Store ID
* Store Location
* Product ID
* Unit Price
* Product Category
* Product Type
* Product Detail

Additional fields were created in the analysis workbook to support the dashboard, including:

* Total Bill
* Month
* Month Name
* Day Name
* Hour
* Size
* Day of Week

---

## 🛠️ Tools & Techniques Used

### Tool

* Microsoft Excel

### Excel Features

* Data Cleaning & Preparation
* Excel Tables
* Pivot Tables
* Pivot Charts
* Slicers
* Calculated Columns
* Data Aggregation
* Data Visualization
* Interactive Dashboard

---

## 🧹 Data Preparation

The raw transaction data was prepared for analysis by creating additional fields required for the dashboard.

The analysis workbook includes calculated fields for:

* **Total Bill** — calculated from transaction quantity and unit price
* **Month Name** — extracted from transaction date
* **Day Name** — extracted from transaction date
* **Hour** — extracted from transaction time
* **Day of Week** — used for weekday analysis
* **Month** — used for chronological monthly analysis
* **Size** — used for order size distribution

These fields were then used to build Pivot Tables and visualizations.

---

## 📊 Dashboard

The final dashboard provides an interactive overview of coffee shop sales performance.

### Dashboard Preview

![Coffee Shop Sales Dashboard](dashboard.png)

### Dashboard KPIs

The dashboard displays:

* **Total Revenue:** €698,812.33
* **Total Transactions:** 149,116
* **Average Order Value:** €4.69
* **Average Items / Order:** 1.44
* **Average Selling Price:** €3.26
* **Total Quantity Sold:** 214,470

### Interactive Filters

The dashboard includes filters for:

* Month
* Day

These filters allow the user to explore sales performance for different periods.

---

# 🔍 Analysis & Findings

## 1. Sales by Hour

Sales activity is strongly concentrated in the morning.

The highest quantity of items sold occurs at **10 AM**, with **26,713 items** sold.

The next strongest hours are:

|  Hour | Quantity Sold |
| ----: | ------------: |
| 10 AM |        26,713 |
|  9 AM |        25,370 |
|  8 AM |        25,197 |
|  7 AM |        19,449 |

After the morning peak, sales activity drops considerably.

### Insight

The **8 AM to 10 AM period is the busiest part of the day**, making morning operations particularly important for staffing, inventory availability, and service efficiency.

---

## 2. Sales by Day of the Week

Transaction activity remains relatively consistent throughout the week.

| Day       | Transactions |     Revenue |
| --------- | -----------: | ----------: |
| Sunday    |       21,096 |  €98,330.31 |
| Monday    |       21,643 | €101,677.28 |
| Tuesday   |       21,202 |  €99,455.94 |
| Wednesday |       21,310 | €100,313.54 |
| Thursday  |       21,654 | €100,767.78 |
| Friday    |       21,701 | €101,373.00 |
| Saturday  |       20,510 |  €96,894.48 |

**Friday** has the highest number of transactions, while **Saturday** has the lowest.

### Insight

The difference between the weekdays is relatively small, suggesting that customer activity is fairly consistent throughout the week. However, Saturday shows the lowest transaction volume and may be worth investigating.

---

## 3. Monthly Revenue

Revenue increases significantly throughout the six month period.

| Month    |     Revenue |
| -------- | ----------: |
| January  |  €81,677.74 |
| February |  €76,145.19 |
| March    |  €98,834.68 |
| April    | €118,941.08 |
| May      | €156,727.76 |
| June     | €166,485.88 |

**June** recorded the highest revenue at **€166,485.88**, while **February** recorded the lowest at **€76,145.19**.

### Insight

The overall pattern shows strong growth from February through June, with May and June showing particularly high sales performance.

---

## 4. Store Location Performance

The three store locations have relatively similar revenue levels.

| Store Location  |     Revenue | Transactions |
| --------------- | ----------: | -----------: |
| Hell's Kitchen  | €236,511.17 |       50,735 |
| Astoria         | €232,243.91 |       50,599 |
| Lower Manhattan | €230,057.25 |       47,782 |

**Hell's Kitchen** generated the highest revenue, while **Lower Manhattan** generated the lowest.

### Insight

The revenue difference between the three locations is relatively small, indicating that overall sales performance is fairly balanced across the stores.

---

## 5. Best Selling Products by Revenue

The top products by revenue are:

| Product               |    Revenue |
| --------------------- | ---------: |
| Barista Espresso      | €91,406.20 |
| Brewed Chai Tea       | €77,081.95 |
| Hot Chocolate         | €72,416.00 |
| Gourmet Brewed Coffee | €70,034.60 |
| Brewed Black Tea      | €47,932.00 |

**Barista Espresso** is the highest revenue product, generating **€91,406.20**.

### Insight

High performing products such as Barista Espresso, Brewed Chai Tea, and Hot Chocolate make a significant contribution to overall revenue and should receive attention when planning inventory and availability.

---

## 6. Best Selling Products by Quantity

The products with the highest quantity sold are:

| Product               | Quantity Sold |
| --------------------- | ------------: |
| Brewed Chai Tea       |        26,250 |
| Gourmet Brewed Coffee |        25,973 |
| Barista Espresso      |        24,943 |
| Brewed Black Tea      |        17,462 |
| Hot Chocolate         |        17,457 |

**Brewed Chai Tea** has the highest quantity sold at **26,250 units**.

### Insight

The product with the highest sales revenue is not necessarily the product with the highest quantity sold.

For example:

* **Barista Espresso** → highest revenue
* **Brewed Chai Tea** → highest quantity sold

This difference highlights the importance of analyzing both **quantity and revenue** when evaluating product performance.

---

## 7. Sales by Product Category

The largest product categories by revenue are:

| Category           |     Revenue | Share of Sales |
| ------------------ | ----------: | -------------: |
| Coffee             | €269,952.45 |         38.63% |
| Tea                | €196,405.95 |         28.11% |
| Bakery             |  €82,315.64 |         11.78% |
| Drinking Chocolate |  €72,416.00 |         10.36% |
| Coffee Beans       |  €40,085.25 |          5.74% |

Coffee is the largest category, contributing approximately **38.63% of total sales**.

Coffee and Tea together contribute approximately **66.74% of total revenue**.

### Insight

Coffee and Tea are the dominant categories in the dataset and represent the largest sources of sales revenue.

---

## 8. Order Size Distribution

The dashboard also shows the distribution of orders by size.

| Size | Orders | Share of Orders |
|---|---:|---:|
| Regular | 45,789 | 30.71% |
| Large | 44,885 | 30.10% |
| Standard / Not Defined | 44,518 | 29.85% |
| Small | 13,924 | 9.34% |

Regular and Large orders represent the largest shares among products with defined size options.

A significant portion of orders is shown as **"Not Defined"**. This does not necessarily indicate missing or incorrect data. Some products in the dataset **do not have different size options**, so they are sold as a standard size. These products are therefore recorded without a specific size such as Small, Regular, or Large.

### Insight

Regular and Large orders account for the largest shares among products with defined size options. The relatively high proportion of **Standard / Not Defined** orders is expected because certain products are not size based.

Therefore, the **"Not Defined"** category should be interpreted as **products without applicable size variations**, rather than as missing data.

---

# 💡 Key Insights

The major findings from the analysis are:

1. **Coffee is the largest product category**, contributing 38.63% of total sales.
2. **Coffee and Tea together contribute approximately 66.74% of total revenue.**
3. **Barista Espresso generates the highest revenue** among the product types.
4. **Brewed Chai Tea has the highest quantity sold.**
5. **10 AM is the busiest hour** based on quantity sold.
6. **Friday has the highest number of transactions**, while Saturday has the lowest.
7. **June is the strongest month** in terms of revenue, generating €166,485.88.
8. **Hell's Kitchen generates the highest store revenue**, although the three stores perform relatively similarly.

---

# 🎯 Recommendations

Based on the observed patterns, the following actions could be considered:

* **Maintain availability of high performing products** such as Barista Espresso, Brewed Chai Tea, and Hot Chocolate.
* **Focus on morning operations**, particularly around the 8 AM to 10 AM period when customer activity is highest.
* **Investigate Saturday performance** to understand why transaction volume is lower than on other days.
* **Study the growth from February to June** to identify factors contributing to the increase in sales.
* **Monitor high performing categories**, particularly Coffee and Tea, because together they contribute approximately two thirds of total revenue.
* **Compare store level operations** to identify practices that could help improve the performance of the lower performing location.

---

# 📁 Project Files

```text
Coffee-Shop-Sales-Analysis/
│
├── Coffee Shop Sales Dashboard.xlsx
├── Dataset.xlsx
├── README.md
└── dashboard.png
```

### File Description

| File                                   | Description                                                             |
| ------------------------               | ----------------------------------------------------------------------- |
| `Dataset.xlsx`                         | Original coffee shop transaction dataset                                |
| `Coffee Shop Sales Dashboard.xlsx`     | Excel workbook containing data preparation, Pivot Tables, and dashboard |
| `dashboard.png`                        | PNG preview of the final dashboard                                      |
| `README.md`                            | Complete project documentation and analysis                             |

---

# ▶️ How to Use

1. Download `Coffee Shop Sales Dashboard.xlsx`.
2. Open the workbook using Microsoft Excel.
3. Go to the **Dashboard** sheet.
4. Use the **Month** and **Day** slicers to filter the dashboard.
5. Explore the KPIs and visualizations.
6. Review the Pivot Tables in the workbook for supporting analysis.

---

# 📝 Conclusion

This project demonstrates how **Microsoft Excel can be used to transform raw transaction data into an interactive dashboard and generate actionable business insights**.

The analysis identifies important patterns in sales by **time, day, month, store location, product, and product category**.

The findings show that **morning hours, Coffee and Tea categories, and several high performing products are major contributors to sales performance**, while areas such as Saturday activity and undefined order size records provide opportunities for further investigation.

Overall, the project combines **data preparation, analysis, visualization, and business interpretation** to provide a structured view of coffee shop sales performance.
