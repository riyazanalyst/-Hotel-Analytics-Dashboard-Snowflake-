# 🏨 Hotel Booking Analytics Dashboard (Snowflake)

An end-to-end **Hotel Booking Analytics Dashboard** built using **Snowflake**, showcasing data ingestion, cleaning, transformation, aggregation, and reporting using **Snowflake Snowsight Dashboards**.

This project demonstrates how raw hotel booking data can be transformed into **business-ready KPIs and insights** using the **Bronze → Silver → Gold** data architecture.

---

## 📌 Project Overview

Hotels often receive booking data in a raw and inconsistent format, making it difficult to answer key business questions such as:
- How much revenue are we generating?
- How many bookings do we receive each month?
- Which cities and room types perform best?
- What is the booking status distribution?

This project solves these problems by building a **fully automated analytics pipeline in Snowflake**, ending with an interactive dashboard for decision-makers.

---

## 🎯 Business Objectives

- Clean and standardize raw booking data  
- Track **total revenue, bookings, and guests**
- Analyze **monthly booking and revenue trends**
- Identify **top revenue-generating cities**
- Understand booking behavior by:
  - Booking status
  - Room type
- Provide management with **quick, reliable KPIs**

---

## 🏗️ Data Architecture

The project follows a **layered data model** widely used in real-world data platforms.

### 🟤 Bronze Layer
- Raw CSV booking data loaded into Snowflake
- Minimal transformation
- Acts as the source of truth

### ⚪ Silver Layer
- Cleaned and standardized data
- Fixed data types (dates, numeric values)
- Removed invalid records
- Handled missing and inconsistent values

### 🟡 Gold Layer
- Aggregated, analytics-ready tables
- Optimized for dashboards and reporting
- Used directly by Snowflake dashboards

---

## 📊 Dashboard Overview

The **Hotel Booking Dashboard** is built using **Snowflake Snowsight** and includes the following components:

### 🔹 Key KPIs
- **Total Guests**
- **Total Bookings**
- **Total Revenue**
- **Average Booking Value**

---

### 🔹 Analytical Visuals

- **Top Cities by Revenue** (Bar Chart)  
- **Bookings by Status** (Confirmed, Cancelled, No-Show)  
- **Bookings by Room Type** (Deluxe, Suite, Standard)  
- **Monthly Bookings Trend** (Line Chart)  
- **Monthly Revenue Trend** (Line Chart)

These visuals provide both **high-level summaries** and **detailed breakdowns** for better decision-making.

---

## 🧰 Tools & Technologies Used

- **Snowflake** – Cloud Data Warehouse  
- **SQL** – Data cleaning, transformation, and aggregation  
- **Snowflake Snowsight Dashboards** – Visualization and reporting  

---

## 📁 Project Structure

hotel-booking-analytics/
│
├── data/
│ └── hotel_bookings.csv
│
├── sql/
│ ├── bronze/
│ │ └── load_bronze.sql
│ │
│ ├── silver/
│ │ └── transform_silver.sql
│ │
│ └── gold/
│ ├── agg_daily_booking.sql
│ ├── agg_city_revenue.sql
│ └── booking_metrics.sql
│
├── dashboard/
│ └── dashboard_queries.sql
│
└── README.md



---

## 🔄 Data Flow

1. Load raw CSV data into **Bronze tables**
2. Clean and standardize data in **Silver tables**
3. Aggregate business metrics in **Gold tables**
4. Build KPIs and visuals using **Snowflake dashboards**

---

## 🧠 Key Learnings

- Practical implementation of **Bronze–Silver–Gold architecture**
- Handling dirty data using:
  - `TRY_TO_DATE`
  - `TRY_TO_NUMBER`
- Designing KPIs for business users
- Understanding Snowflake:
  - Warehouses
  - Roles
  - Dashboard execution behavior
- Difference between Snowflake dashboards and BI tools like Power BI

---

## 🚀 Outcome

This project delivers a **production-style analytics solution** that enables hotel management to:
- Monitor revenue and bookings in real time
- Identify top-performing cities and room types
- Understand booking behavior and cancellations
- Make faster, data-driven decisions

---

## 📌 Future Enhancements

- Add incremental data loading using **Streams & Tasks**
- Create a dedicated `GOLD` schema
- Add advanced KPIs (Cancellation Rate, Revenue per Guest)
- Connect Snowflake to Power BI or Tableau
- Implement automated data quality checks

---

## 👤 Author

**Mohammed Riyaz**  
Data Analyst | Snowflake | SQL | Power BI  

---

⭐ If you found this project useful, feel free to star the repository!
