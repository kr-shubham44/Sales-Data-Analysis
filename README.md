# 🧮 Sales Data Analysis (Python Project)

## 📘 Overview
This project analyzes sales performance using the **Sample Superstore Dataset**.  
The goal is to identify insights such as regional sales patterns, profit distribution, and month-wise trends.

---

## 🧰 Tools & Libraries Used
- **Python**
- **Pandas** – for data cleaning and analysis  
- **Matplotlib** – for data visualization  
- **Seaborn** – for advanced visual charts  

---

## 📊 Project Workflow

### 1️⃣ Data Cleaning
- Handled **missing values** and **duplicates**
- Converted date columns (`Order Date`, `Ship Date`) to datetime format
- Verified data types and formatted numeric columns

### 2️⃣ Exploratory Data Analysis (EDA)
- Calculated **total sales**, **profit**, and **discount**      
- Grouped data by:
  - Region
  - Category
  - Sub-Category
- Identified **top-performing regions and categories**

### 3️⃣ Visualization
Created clear and attractive charts:
- 📈 **Month-wise sales trend**
- 📊 **Region-wise sales comparison**
- 🧩 **Category-wise profit distribution**

### Example Code Snippet:
```python
region_sales = df.groupby('Region')['Sales'].sum().sort_values(ascending=False)
plt.bar(region_sales.index, region_sales.values)
plt.title('Region-wise Sales')
plt.xlabel('Region')
plt.ylabel('Total Sales')
plt.show()
