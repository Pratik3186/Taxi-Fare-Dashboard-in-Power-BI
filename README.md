# 🚖 Taxi Fare Dashboard in Power BI

## 📊 Project Overview

The **Taxi Fare Dashboard** is a comprehensive Power BI project designed to analyze ride-booking data and extract meaningful business insights. It provides a complete overview of ride performance, revenue trends, customer behavior, cancellations, and service quality.

This dashboard helps stakeholders make **data-driven decisions** by visualizing key metrics across multiple dimensions such as time, vehicle type, payment method, and customer segments.

---

## 🎯 Objectives

* Analyze booking trends over time
* Understand revenue distribution and growth
* Evaluate cancellation patterns
* Measure service quality and customer retention
* Compare performance across vehicle types
* Identify peak vs off-peak business performance

---

## 🧾 Dataset Description

The dataset contains ride-booking information with the following key attributes:

* Booking ID
* Date & Time
* Booking Status (Completed, Cancelled, etc.)
* Booking Value
* Customer ID
* Driver Ratings & Customer Ratings
* Vehicle Type
* Payment Method
* Distance Travelled

---

## 📌 Dashboard Pages

### 🏠 Homepage

* Navigation panel for all dashboard sections
* Clean UI for seamless user experience

---

### 📈 Overall Analysis

* Total bookings count (~148K+)
* Monthly booking trends
* Booking status distribution
* Driver cancellation insights 

---

### 🚗 Vehicle Type Analysis

* Total booking value by vehicle
* Successful bookings
* Average distance travelled
* Total distance metrics

---

### 💰 Revenue Analysis

* Revenue by payment method (UPI, Cash, Cards, Wallet)
* Revenue per KM by vehicle type
* Daily ride distance trends
* Revenue contribution breakdown

---

### ❌ Cancellation Analysis

* Cancellation reasons (Customer & Driver)
* Cancellation percentage (~25%)
* Behavioral insights on failed rides

---

### ⭐ Ratings Analysis

* Customer vs Driver ratings comparison
* Performance distribution across vehicle types

---

### 📊 Summary Dashboard

* Key KPIs:

  * 💵 Total Revenue: **3.86M**
  * 📈 Premium Peak Hour Index: **72.53%**
  * 🔁 Customer Retention Rate: **30.24%**
  * ⭐ Service Quality Score: **77.05** 

* Revenue segmentation:

  * Premium / High / Medium / Low

* Time-based insights:

  * Morning / Afternoon / Evening / Night

* Trend analysis:

  * Monthly Revenue
  * Weekly Bookings

---

## 🧠 Key DAX Measures

### 🔹 Service Quality Score

* Combines driver ratings, completion rate, and cancellation rate

### 🔹 Customer Retention Rate

* Identifies repeat customers with multiple completed rides

### 🔹 Premium Peak Hour Index

* Compares peak vs off-peak revenue

### 🔹 Monthly Revenue

* Rolling 30-day revenue calculation

### 🔹 Weekly Bookings

* Rolling 7-day booking trend

### 🔹 Quarterly Avg Booking Value

* Average booking value over last 3 months

### 🔹 Revenue Tier (Calculated Column)

```DAX
Revenue_Tier =
SWITCH(
    TRUE(),
    rideBookings[Booking Value] >= 500, "Premium",
    rideBookings[Booking Value] >= 200, "High",
    rideBookings[Booking Value] >= 100, "Medium",
    "Low"
)
```

---

## 📊 Key Insights

* 📈 Peak hours (6–9 AM & 5–9 PM) generate higher revenue
* 🚖 Auto and Go Mini contribute major revenue share
* 💳 UPI is the most preferred payment method
* ❌ ~25% rides get cancelled → optimization opportunity
* 🔁 Customer retention is relatively low (~30%)
* ⭐ Service quality score indicates moderate performance

---

## ⚙️ Tools & Technologies

* **Power BI Desktop**
* **DAX (Data Analysis Expressions)**
* Data Modeling & Visualization

---

## 🚀 How to Use

1. Download the `.pbix` file
2. Open in Power BI Desktop
3. Explore different pages using navigation panel
4. Use filters (Date, Vehicle Type, Payment Category, Day Part)

---

## 📷 Dashboard Preview

(Add screenshots here from your PDF)

---

## 📌 Future Improvements

* Add predictive analytics (forecasting demand)
* Integrate real-time data streaming
* Implement customer segmentation using ML
* Optimize cancellation prediction

---

## 👨‍💻 Author

**Pratik**

* Aspiring Data Analyst & Developer
* Focused on building real-world data-driven projects

---

## ⭐ If you like this project

Give it a ⭐ on GitHub and share feedback!

---
