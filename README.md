# Logistic & Delivery Time Optimization

## 📌 Project Overview

This project focuses on analyzing logistics and delivery data to **optimize delivery time, reduce delays, and improve operational efficiency**.
The analysis transforms raw logistics data into meaningful insights using **Python for data preprocessing** and **Power BI for visualization and KPI analysis**.

The goal is to support **data-driven logistics decision-making** by identifying delay patterns, cost drivers, and performance gaps across cities, transport modes, and warehouses.

---

## 🎯 Business Objectives

* Measure overall delivery performance using key KPIs
* Identify causes of delivery delays
* Analyze delivery time across cities and transport modes
* Evaluate shipping cost efficiency by distance and transport mode
* Enable interactive analysis for logistics stakeholders

---

## 📂 Dataset Description

The dataset contains logistics shipment records where each row represents a single order.

### Key Attributes:

* Order, Dispatch, and Delivery Dates
* Origin and Destination Cities
* Distance (km)
* Transport Mode (Air, Road, Rail, Sea)
* Shipment Weight and Shipping Cost
* Delivery Status (Early, On Time, Delayed)
* Delay Reason
* Customer Rating

---

## 🛠 Tools & Technologies Used

* **Python** (Pandas, NumPy) – Data cleaning & feature engineering
* **Power BI** – KPI dashboards & interactive analysis

---

## 🧹 Data Preprocessing (Python)

Python was used to clean and prepare real-world logistics data before visualization:

### Key Steps:

* Loaded raw CSV data using Pandas
* Inspected dataset structure, data types, and size
* Converted date columns (Order, Dispatch, Delivery) into proper datetime format
* Handled missing values:

  * Filled missing delay reasons with `"None"`
  * Replaced missing customer ratings with median values
  * Removed rows with missing critical dates
* Removed duplicate records to ensure accurate order counts
* Validated date logic:

  * Delivery Date ≥ Dispatch Date ≥ Order Date
* Engineered new features:

  * **Delivery_Time_Days** (Delivery Date – Dispatch Date)
  * **Is_Delayed** flag (1 = Delayed, 0 = Not Delayed)
* Generated summary statistics to inspect outliers
* Exported the cleaned dataset for Power BI analysis 

---

## 📊 Key Performance Indicators (KPIs)

* **Average Delivery Time (Days)**
* **Total Orders Processed**
* **Delay Percentage**

These KPIs provide a quick overview of logistics efficiency and service reliability .

---

## 🔍 Key Analysis & Insights

### 🚚 Delivery Time by Destination City

* Cities like **Kolkata and Coimbatore** show higher average delivery times
* **Ahmedabad** has the lowest average delivery time
* Indicates city-level operational differences that require optimization 

---

### 💰 Shipping Cost vs Distance & Transport Mode

* **Air transport** has the highest shipping cost, especially for long distances
* **Road and Rail** are cost-effective for short and medium distances
* **Sea transport** is most economical for long-distance shipments
* Helps in selecting optimal transport modes to reduce costs 

---

### ⏱ Delivery Time by Transport Mode

* **Rail** has the highest average delivery time
* **Road transport** performs better in speed and reliability
* **Sea transport** shows the lowest average delivery time in the dataset
* Highlights transport mode efficiency differences 

---

### ⚠ Delay Reason Analysis

* Major contributors to delays:

  * Mechanical issues
  * Warehouse delays
  * Traffic and weather conditions
* Identifies operational areas requiring immediate attention 

---

### 📦 Delivery Status Distribution

* Most orders are delivered **Early** or **On Time**
* Delayed orders are fewer but still significant
* Provides an overall view of service punctuality and reliability 

---

## 🎛 Interactive Dashboard Features

Power BI dashboard includes slicers for:

* Warehouse ID
* Delivery Status (Early / On Time / Delayed)
* Transport Mode

These filters allow stakeholders to drill down into specific operational scenarios and perform root-cause analysis .

---

## 📈 Business Recommendations

* Optimize transport mode selection based on distance and urgency
* Improve warehouse operations to reduce internal delays
* Address mechanical and traffic-related issues proactively
* Monitor city-level delivery performance regularly
* Use KPI tracking to continuously improve logistics efficiency 

---

## ✅ Conclusion

This project demonstrates how **Python-based data preprocessing** combined with **Power BI dashboards** can uncover inefficiencies in logistics operations.
By identifying delay causes, cost drivers, and performance gaps, the analysis enables smarter logistics planning and improved delivery performance.

---

## 📚 Learning Outcomes

* Practical data cleaning and feature engineering using Python
* Time-based logistics analysis
* KPI-driven dashboard design
* Business-focused storytelling with data

