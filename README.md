# Travvise Flight Booking Analytics Dashboard

## Project Overview
The Travvise Flight Booking Analytics Dashboard is a Power BI project designed to analyze and monitor flight booking data. The dashboard provides insights into ticket booking trends, supplier performance, airline distribution, destination popularity, and company-level performance.

The report consists of multiple interactive pages that allow users to explore ticket booking data across different dimensions such as companies, suppliers, airlines, and time periods. This helps stakeholders understand booking behavior, identify key business contributors, and make informed decisions.

---

## Purpose of the Project
The main objective of this dashboard is to provide a centralized and interactive view of flight booking performance. It enables users to:

- Monitor total ticket bookings
- Compare weekday and weekend ticket trends
- Analyze company-level booking performance
- Identify top destinations and airlines
- Evaluate supplier distribution
- Track ticket lifecycle events like issued, cancelled, refunded, and void tickets

This helps travel management teams and business stakeholders identify key opportunities and optimize booking strategies.

---

## Tech Stack

- **Power BI** – Data visualization and dashboard development  
- **SQL** – Data extraction from the database  
- **Power Query** – Data cleaning and transformation  
- **DAX (Data Analysis Expressions)** – Creating calculated measures and KPIs  
- **Data Modeling** – Building relationships between tables for analysis  

---

## Data Source

The dataset used in this project is sourced from a **SQL database containing flight booking transaction data**.

---

Below is a brief description of the key tables used in the data model.

### Company
Contains information about companies that book flight tickets.

### CompBranch
Stores branch-level details for each company.

### CustomerUser
Contains details of users who perform flight searches and bookings.

### Supplier
Stores information about travel suppliers or booking providers.

### SupplierType
Classifies suppliers into categories such as GDS, NDC, or LCC.

### FlightSearch
Contains details of flight search queries including airline, cabin type, and destination.

### Flight Search Response
Stores the response results returned from flight search requests.

### FlightTransactions
Contains booking transaction information for flight tickets.

### FlightTransactionDetails
Stores detailed information about ticket transactions.

### FlightTransactionSegmentDetails
Contains flight segment information such as origin, destination, and airline.

### View_Flighttransaction
A view table used to consolidate flight transaction information for reporting.

### View_Flighttransaction_SegmentDetails
A view table that provides detailed flight segment data for analysis.

### Ticket
Stores ticket-related booking data.

### Ticket Count
Contains aggregated ticket count information used for KPIs.

---

# Report Pages

## Executive View
This page provides a high-level overview of the overall flight booking performance.

Key insights include:

- **Total Ticket Count**
- **Weekend Ticket Count**
- **Weekday Ticket Count**
- **Monthly Ticket Trend Analysis**
- **Top 10 Origin Locations**
- **Top 10 Destinations**
- **Top 10 Companies by Ticket Count**
- **Top Airlines by Ticket Count**
- **Ticket Count by Supplier Type (GDS, NDC, LCC)**

Interactive filters allow users to analyze the data by:

- Company
- Country
- Supplier Type
- Supplier
- Year
- Quarter
- Month

This page acts as the **executive summary for booking performance and travel demand patterns**.

---

## Company Performance
This page focuses on analyzing **ticket bookings at the company level**.

Key features include:

- **Company-wise Ticket Count**
- **Year-over-Year (YoY) Change**
- **YoY Growth Percentage**
- **Comparison between Current Year and Previous Year**
- **Company Performance Trend Over Time**

Visuals included:

- Company performance table with YoY comparison
- Monthly performance trend chart
- Ticket count comparison across companies
- Supplier type distribution

This page helps identify **top-performing companies and track their booking growth trends**.

---

## Ticket Count View
This page analyzes the **ticket lifecycle and booking flow across different entities**.

Key metrics displayed:

- **Issued Tickets**
- **Reissued Tickets**
- **Refunded Tickets**
- **Cancelled Tickets**
- **Void Tickets**

It also includes a **drill-down flow visualization** showing how ticket counts move across different dimensions:

Ticket Count → Company → Registered Company → Supplier Type → Supplier → Airline Code

This helps analyze **how bookings are distributed across companies, suppliers, and airlines**.

---

## Interactive Features

Users can dynamically explore the dashboard using filters such as:

- Company
- Country
- Supplier Type
- Supplier
- Airline
- Year
- Quarter
- Month

These filters allow deeper exploration and help users focus on specific segments of the booking data.

---

## Key Insights Provided

- Comparison of weekday vs weekend booking trends
- Identification of top travel destinations
- Analysis of airline booking distribution
- Company-level performance tracking
- Supplier channel analysis
- Monitoring ticket lifecycle events (issued, cancelled, refunded, etc.)

---
# Dashboard Preview

### Executive View
[Travvise_Analytics.PNG](https://github.com/Parul13github/POWER-BI_TRAVVISE-ANALYTICS/blob/main/Travvise_Analytics.PNG)

### Company Performance
https://github.com/Parul13github/POWER-BI_TRAVVISE-ANALYTICS/blob/main/Travvise_Analytics_Company%20Performance.PNG

### Ticket Count View
https://github.com/Parul13github/POWER-BI_TRAVVISE-ANALYTICS/blob/main/Travvise_Analytics_TicketCountView.PNG

---

## Project Files

- `Travvise_Consolidated_Analytics.pbit` – Power BI dashboard file
