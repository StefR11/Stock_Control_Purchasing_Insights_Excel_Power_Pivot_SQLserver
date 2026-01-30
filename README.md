This repository contains a Purchasing Insights analytics project developed from real operational data extracted from a hotel stock control system.
The dataset consists of approved purchase invoices for the entire year of 2025, analysed using Excel (Power Pivot) and SQL Server.

The objective of the project is to:

Monitor purchasing performance

Identify spend concentration and supplier dependency

Detect operational inefficiencies

Analyse demand trends over time

DATA PREPARATION

Exported approved purchase invoices (2025) from the stock control system into Excel

Cleaned and transformed the data using Power Query, including:

Standardising tables and fields

Creating a new classification column to distinguish Food vs Beverage purchases

Loaded the data into the Excel Data Model for advanced analysis

EXCEL DATA MODELS & MEASURES

Using DAX measures, the following KPIs were created:

Total Purchases

Transaction Count

MTD, QTD, YTD Purchases & Transactions

% of Total Purchases

Previous Month Purchases & Transactions

Month-over-Month Difference and % Change

60-Day Rolling Total (Purchases & Transactions)

60-Day Rolling Average

Daily Cumulative Purchases & Transactions

DASHBOARD

The Excel dashboard is built using:

Pivot tables

Conditional formatting

Timeline slicer

The dashboard provides a clear view of purchasing behaviour across time, suppliers, and product categories.

KEY INSIGHTS

Food purchases significantly outweigh beverage purchases, indicating inefficiencies in beverage invoice approval and stock control processes

Top 3 suppliers by total spend are meat, vegetables, and dairy suppliers

Fish suppliers rank lower (6th by total spend), suggesting either lower guest demand for fish or a menu skewed towards meat

Brake & Bros, primarily used for staff food, ranks 4th in total spend despite limited weekly deliveries — highlighting potential overspending on staff meals

A strong increase in total purchases during Q4 indicates rising workload and guest numbers toward year-end

SQL SERVER ANALYSIS

In parallel, all major Excel measures were replicated in SQL Server, focusing on:

Query combination and transformation

ALTER and UPDATE statements

CTEs

Joins

Window functions

Aggregations and subqueries

This allowed validation of Excel results and strengthened understanding of how time-based and rolling KPIs can be calculated directly in SQL.

REPOSITORY CONTENTS

📊 Excel Pivot Table Dashboard

🧮 SQL Server queries replicating business KPIs
