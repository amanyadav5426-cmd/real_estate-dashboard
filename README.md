# 🏠 Real Estate Market & Investment Intelligence

An end-to-end **Business & Data Analytics project** that analyzes real-estate transaction data to identify property-market trends, pricing patterns, locality performance, and potential investment opportunities.

The project simulates the work of a **Data Analyst supporting a real-estate firm's business and investment decisions**.

---

## 🎯 Business Problem

Real-estate companies deal with large volumes of property and transaction data, but raw data alone does not provide clear answers to important business questions.

This project aims to answer:

* Which localities have the highest property values?
* Which property types generate the highest transaction value?
* How does property size affect sale price?
* Which locations have the highest price per square foot?
* Are properties selling above or below their estimated value?
* Which property segments represent potential market opportunities?
* How have transaction values changed over time?

The goal is to transform raw property data into **actionable business insights**.

---

## 📊 Project Objectives

1. Clean and prepare real-estate transaction data.
2. Perform exploratory and descriptive analysis using Excel.
3. Store and analyze structured data using PostgreSQL.
4. Use SQL to answer real-world business questions.
5. Build an interactive Power BI dashboard.
6. Identify pricing and market trends.
7. Translate analytical findings into business recommendations.

---

## 🛠️ Tools & Technologies

| Tool                | Purpose                                            |
| ------------------- | -------------------------------------------------- |
| **Kaggle**          | Source of real-estate transaction data             |
| **Microsoft Excel** | Data cleaning, transformation and initial analysis |
| **PostgreSQL**      | Data storage and SQL analysis                      |
| **SQL**             | Business queries and analytical calculations       |
| **Power BI**        | Interactive dashboard and visualization            |
| **DAX**             | Business metrics and Power BI calculations         |
| **GitHub**          | Project documentation and version control          |

**Python is not used in this project.**

---

## 🔄 Project Workflow

```text
Kaggle Dataset
      ↓
Excel / Power Query
      ↓
Data Cleaning & Transformation
      ↓
PostgreSQL
      ↓
SQL Business Analysis
      ↓
Power BI + DAX
      ↓
Interactive Dashboard
      ↓
Business Insights
      ↓
Recommendations
```

---

## 📁 Project Structure

```text
Real-Estate-Market-Investment-Intelligence/
│
├── Data/
│   ├── raw_data/
│   └── cleaned_data/
│
├── Excel/
│   └── real_estate_analysis.xlsx
│
├── SQL/
│   ├── 01_database_setup.sql
│   ├── 02_data_exploration.sql
│   ├── 03_basic_metrics.sql
│   ├── 04_locality_analysis.sql
│   ├── 05_property_analysis.sql
│   ├── 06_price_analysis.sql
│   ├── 07_time_analysis.sql
│   ├── 08_advanced_analysis.sql
│   └── 09_business_questions.sql
│
├── PowerBI/
│   └── real_estate_dashboard.pbix
│
├── Screenshots/
│   └── dashboard.png
│
└── README.md
```

---

## 🧹 Data Cleaning — Excel

The raw Kaggle dataset was prepared for analysis using Excel and Power Query.

Key data-preparation activities include:

* Removing duplicate records
* Handling missing values
* Standardizing categorical values
* Correcting data types
* Validating numerical fields
* Checking invalid property values
* Standardizing date formats
* Creating calculated business metrics

### Calculated Metrics

Examples include:

**Price per Square Foot**

```text
Sale Price / Area
```

**Price Difference**

```text
Actual Sale Price - Estimated Value
```

**Price Difference %**

```text
((Actual Sale Price - Estimated Value) / Estimated Value) × 100
```

---

## 📈 Excel Analysis

Excel was used to perform initial business analysis using:

* PivotTables
* PivotCharts
* Slicers
* Conditional Formatting
* XLOOKUP
* SUMIFS
* COUNTIFS
* AVERAGEIFS
* IF / IFS
* Power Query

The analysis focuses on:

* Locality performance
* Property-type performance
* Price distribution
* Property size
* Price per square foot
* Estimated vs actual sale value
* Transaction trends

---

## 🗄️ PostgreSQL & SQL Analysis

The cleaned dataset was imported into PostgreSQL for structured querying and deeper analysis.

SQL techniques used include:

* `SELECT`
* `WHERE`
* `GROUP BY`
* `HAVING`
* `ORDER BY`
* Aggregate functions
* `CASE`
* `JOIN`
* CTEs
* Subqueries
* Window functions
* Ranking
* Analytical views

### Example Business Query

```sql
SELECT
    locality,
    COUNT(*) AS total_transactions,
    AVG(sale_price) AS average_sale_price
FROM properties
GROUP BY locality
ORDER BY average_sale_price DESC;
```

This identifies localities with the highest average transaction prices.

---

## 📊 Power BI Dashboard

The final dashboard provides an interactive view of the real-estate market.

### Key KPIs

* Total Transactions
* Total Sales Value
* Average Sale Price
* Median Sale Price
* Average Price per Sq. Ft.
* Average Property Area

### Dashboard Analysis

The dashboard covers:

**Market Overview**

* Transaction volume
* Total sales value
* Price trends

**Locality Intelligence**

* Average price by locality
* Price per sq. ft.
* Locality comparison

**Property Intelligence**

* Property type
* Rooms/BHK
* Property size
* Pricing patterns

**Valuation Analysis**

* Estimated vs actual sale price
* Properties selling above/below estimated value

Interactive filters allow users to explore the data by relevant dimensions such as locality, property type, rooms/BHK and time period.

---

## 💡 Business Insights

The analysis is designed to identify insights such as:

* Premium localities with higher price per square foot
* Property segments contributing the highest transaction value
* Locations with relatively lower property prices
* Properties selling significantly above or below estimated value
* Changes in transaction activity over time
* Relationship between property characteristics and pricing

The findings are translated into **business recommendations** rather than presenting charts alone.

---

## 🎯 Business Impact

This project demonstrates how a real-estate organization can use analytics to:

* Compare property markets across locations
* Improve pricing decisions
* Identify attractive property segments
* Understand market trends
* Evaluate estimated vs actual property valuations
* Support investment and acquisition decisions

---

## 📌 Key Learning Outcomes

Through this project, the following skills were developed:

* Business problem formulation
* Excel-based data cleaning
* Data validation
* Exploratory data analysis
* Advanced Excel formulas
* PivotTable analysis
* SQL querying
* PostgreSQL data management
* Business KPI development
* Power BI dashboard development
* DAX-based calculations
* Data-driven decision making
* Business storytelling

---

## 🚀 Future Improvements

Possible future enhancements include:

* Adding more recent real-estate transaction data
* Incorporating external economic indicators
* Adding rental yield analysis
* Adding location-level market comparisons
* Building a more advanced investment scoring framework
* Incorporating property demand indicators

---

## 👤 Project Role

**Role:** Data Analyst

Responsibilities included:

* Data preparation and cleaning
* Excel analysis
* SQL-based analysis
* KPI development
* Dashboard development
* Business insight generation
* Recommendation development

---

## 📚 Dataset

**Source:** Kaggle — Real Estate Property Transactions Dataset

The dataset is used for educational and analytical purposes.

---

## ⭐ Conclusion

**Real Estate Market & Investment Intelligence** demonstrates an end-to-end analytics workflow where raw real-estate data is transformed into meaningful insights for business decision-making.

The project combines **Excel, SQL, PostgreSQL and Power BI** to move from raw data to actionable business recommendations.
