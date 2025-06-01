# 🚴‍♂️ Bicycle Purchase Behavior Analysis (Excel Dashboard Project)

## 📌 Project Overview

This Excel-based project explores **consumer purchasing behavior** for bicycles by analyzing demographic and socioeconomic data. The goal is to understand how factors like **gender, income, age, commute distance, car ownership**, and **marital status** influence the decision to purchase a bicycle.

The dataset consists of over **1,000 customer records**, including the following columns:

- Customer ID  
- Gender  
- Marital Status  
- Income  
- Education  
- Occupation  
- Number of Cars Owned  
- Commute Distance  
- Region  
- Age  
- Purchased Bike (Yes/No)

---

## 🎯 Objectives

- Analyze the impact of **demographics** on bike purchase decisions  
- Identify **trends and patterns** across gender, age brackets, income levels, and commute distance  
- Visualize the insights in a clean and interactive **Excel dashboard** using pivot tables and charts

---

## 🧹 Data Cleaning & Preparation (Excel)

The raw data required several preprocessing steps to prepare it for meaningful analysis:

### ✅ Standardization
- Replaced abbreviated values in `Gender` and `Marital Status` (e.g., “M” → “Married”, “F” → “Female”) using Excel’s **Find & Replace**.
- Cleaned and formatted the `Income` column using **TRIM()** and number formatting to ensure consistency.
- Applied proper formatting to all columns to align with their data types.

### ✅ Age Bracketing
To make the `Age` data more useful for analysis, I categorized each entry into defined age groups using the **IFS()** function:

`=IFS(
  L2 > 59, "Senior (60+)",
  L2 >= 45, "Older Adult (45–59)",
  L2 >= 25, "Young Adult (25–44)",
  L2 >= 18, "Youth (18–24)",
  L2 >= 0, "Child (0–17)",
  ISBLANK(L2), "No Data",
  TRUE, "Invalid Age"
)`

## 📊 Analysis via Pivot Tables

I created pivot tables and visual charts to answer key business questions:

- **Gender vs Bike Purchase**: Do men or women buy more bikes?
- **Income vs Purchase Decision**: Does income influence the likelihood of purchasing a bike?
- **Commute Distance vs Purchase**: Do people with shorter or longer commutes buy more bikes?
- **Age Bracket vs Purchase**: Which age group tends to buy more?
- **Car Ownership vs Purchase**: Does owning more cars reduce the likelihood of buying a bike?

---

## 🔍 Key Insights

- **Income**: Individuals who purchased bikes generally earn more, with a difference of approximately **$3,000–$4,000** compared to those who didn’t.
- **Gender**: **Males** are more likely to purchase bicycles than females.
- **Commute Distance**: Customers with a commute distance of **0–5 miles** had the highest bike purchase rates. The likelihood of purchasing a bike drops as commute distance increases beyond 5 miles.
- **Age Bracket**: The **Young Adult (25–44)** age group had the highest rate of bicycle purchases. **Senior (60+)** customers were the least likely to purchase.
- **Car Ownership**: Customers with **0 to 2 cars** were more likely to purchase a bike. Those with **3 or more cars** were significantly less likely to buy one.

---

## 💡 Skills Demonstrated

- Data cleaning and formatting using **Excel**
- Use of logical functions like `IFS()`, `TRIM()` for categorization and cleanup
- Building and interpreting **pivot tables**
- Creating **interactive dashboards** with charts
- Extracting **actionable insights** to support data-driven decisions

---

## 📁 Tools Used

- Microsoft Excel / Google Sheets  
- Pivot Tables  
- Conditional Formatting  
- Charts & Graphs  
- Excel Functions: `IFS()`, `TRIM()`, `REPLACE()`

---

## ✅ Conclusion

This project helped refine my skills in **data cleaning, analysis, and visualization** using Excel. I gained hands-on experience transforming raw customer data into clear insights through dashboards and charts. It reinforced the importance of understanding the data before analysis and communicating findings in a way that supports **effective decision-making**.

You can explore the Excel workbook and dashboard included in this repository for a closer look at the methodology and results.
