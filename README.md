# 🏨 Hotel Analytics Dashboard (Snowflake)

An end-to-end **Hotel Analytics Dashboard** built using **Snowflake**, following the **Bronze → Silver → Gold** data architecture.  
This project focuses on transforming raw booking data into clean, aggregated, and business-ready insights using SQL and Snowflake dashboards.

---

## 📌 Project Overview

The hotel receives booking data in a **raw and inconsistent format**, making it difficult to analyze:
- Monthly revenue
- Booking trends
- City-level performance

This project solves the problem by:
- Cleaning and standardizing raw data
- Transforming data into analytical layers
- Creating business KPIs and visualizations directly in **Snowflake Snowsight**

---

## 🎯 Business Objectives

- Clean and standardize booking data
- Show **monthly revenue** and **monthly bookings**
- Identify **top revenue-generating cities**
- Analyze bookings by **room type** and **booking status**
- Display key KPIs:
  - Total Revenue
  - Total Bookings

---

## 🏗️ Data Architecture (Bronze–Silver–Gold)

### 🟤 Bronze Layer
- Raw CSV files loaded into Snowflake
- No transformations applied
- Acts as the source of truth

### ⚪ Silver Layer
- Cleaned and standardized data
- Correct data types (dates, numbers)
- Invalid records filtered
- Data quality issues handled

### 🟡 Gold Layer
- Aggregated, business-ready tables
- Optimized for reporting and dashboards
- Used directly by Snowflake dashboards

---

## 📊 Dashboard Features

### Visuals
- 📈 Revenue per Month (Line Chart)
- 📈 Bookings per Month (Line Chart)
- 📊 Top Cities by Revenue (Bar Chart)
- 📊 Bookings by Room Type (Bar Chart)
- 📊 Bookings by Booking Status (Bar Chart)

### KPIs
- 💰 Total Revenue
- 📦 Total Bookings

---

## 🧰 Tech Stack

- **Snowflake** – Cloud Data Warehouse  
- **SQL** – Data cleaning, transformation, aggregation  
- **Snowflake Snowsight Dashboards** – Reporting & visualization  

---

## 📁 Project Structure

