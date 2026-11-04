# Fleet_Telematics_Analytics

An end-to-end data pipeline and interactive business intelligence solution engineered to process raw fleet telematics, optimize preventative maintenance schedules, and reduce operational downtime.


## Tech Stack & Architecture

* ETL Pipeline: Python (Pandas, NumPy, SQLAlchemy)
* Data Storage & Integrity: SQL (PostgreSQL / MySQL) with schema validations and window functions
* Data Modeling & Visualization: Power BI (Star-schema relational model, DAX calculations)
* Version Control: Git / GitHub


## Project Overview & Objectives

Managing enterprise fleet logistics requires real-time insight into vehicle utilization, telematics anomalies, and maintenance logs. This project establishes an automated pipeline to ingest messy operational logs, enforce strict data quality checks, and deliver actionable insights via an interactive executive dashboard.

### Core Objectives:
* Automate Data Extraction & Transformation: Clean, normalize, and validate raw sensor and maintenance data.
* Enforce Data Integrity: Execute SQL-based quality checks to identify duplicate telematics records, missing timestamps, and outlier data.
* Deliver Executive Metrics: Calculate fleet reliability metrics such as Mean Time Between Failures (MTBF), Mean Time to Repair (MTTR), total downtime costs, and fuel efficiency trends.


## Key Features & Analysis

1. Python ETL Pipeline:
   * Automated parsing and structured ingestion of raw JSON/CSV telematics logs.
   * Data cleaning script to handle null values, timezone adjustments, and categorical encoding.

2. SQL Relational Model & Quality Checks:
   * Normalized schema designed for fast analytical queries across Vehicles, Trips, Telematics_Events, and Maintenance_Logs.
   * Advanced SQL window functions used to track vehicle metric trends over time.

3. Power BI Interactive Dashboard:
   * Dynamic filtering by vehicle class, date ranges, and fault severity levels.
   * Custom DAX measures for real-time tracking of operational availability rates and scheduled vs. unscheduled downtime.
   

## How to Replicate

1. Clone the Repository:
   git clone https://github.com/YOUR_USERNAME/enterprise-fleet-telematics-analytics.git
   cd enterprise-fleet-telematics-analytics

2. Set Up Python Environment:
   python -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   pip install -r requirements.txt

3. Run the Data Pipeline:
   python etl/clean_telematics.py

4. Explore the Power BI Report:
   Open powerbi/fleet_analytics.pbix in Power BI Desktop to view the data model and visual analytics.
