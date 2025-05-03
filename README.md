# 🚖 NYC Taxi Data Exploratory Analysis

A comprehensive data analysis framework using **Apache Spark** and **Jupyter Notebook** for exploring and analyzing NYC Yellow Taxi trip data.

---

## 📌 Project Overview

This repository provides a Spark-based exploratory data analysis (EDA) of the NYC Yellow Taxi dataset. The analysis focuses on understanding:

- Trip patterns
- Fare structures
- Tipping behavior
- Operational trends
- Urban mobility insights

---

## ⚙️ Approach

### 1. Environment Setup

- Apache Spark and PySpark configured within a Jupyter Notebook environment
- Suitable for both local and distributed (e.g., EMR, Databricks) deployments

### 2. Data Engineering

- **Data Ingestion**: NYC Yellow Taxi data (Jan–Mar 2023) downloaded in Parquet format for efficient Spark-based processing
- **Feature Engineering**:
  - Temporal features (hour, day, month, weekday/weekend)
  - Trip speed, tip percentage, duration
- **Data Cleaning**:
  - Removed trips with invalid or zero distance, fare, or duration
  - Filtered outliers using logical thresholds

### 3. Analysis Components

#### 📅 Temporal Analysis
- Trip count by hour, day of week, and month
- Weekday vs. weekend usage comparison
- Identification of peak demand hours

#### 💰 Financial Analysis
- Fare amount vs. trip distance and duration
- Tipping behavior by time of day and passenger count
- Distribution of tip percentages

#### 🚕 Trip Characteristics
- Distance and duration distribution
- Average and peak speeds by hour
- Categorization of trips (short, medium, long)

#### 🗺️ Geospatial Analysis *(Optional/Future Work)*
- Pickup/dropoff hotspot clustering
- Geographical correlation with fares and trip counts

---

## 📊 Visualization Highlights

Visuals generated via Pandas + Matplotlib/Seaborn (after `.toPandas()` conversion from Spark):

- Trip volume distribution by hour
- Fare amount vs. distance scatter plot
- Tip % vs. time of day
- Correlation heatmaps
- Weekday vs. weekend comparison charts

---

## ❓ Key Exploratory Questions

### 📅 Temporal Patterns
- How do trips vary by hour, weekday, and month?
- Are there behavioral differences in weekdays vs. weekends?
- How has COVID-19 impacted trip patterns (pre/post-pandemic)?
- What are the busiest taxi hours?

### 💸 Financial Insights
- What factors drive fare amount?
- How does tipping vary with time or passenger count?
- Is there a correlation between trip distance and tip percentage?

### 🧭 Operational Insights
- Average speed during rush vs. off-peak hours
- Trip distance distribution (short, medium, long)
- Seasonal patterns in duration and distance
- Breakdown of trip categories:
  - **Short**: 0–2 mi
  - **Medium**: 2–10 mi
  - **Long**: >10 mi

---

## 📂 Repository Structure

```text
nyc-taxi-eda/
├── nyc_taxi_eda.ipynb        # Main Jupyter Notebook for Spark-based EDA
├── nyc_taxi_data/            # Folder to store downloaded Parquet files
├── README.md                 # Project overview and documentation
├── requirements.txt          # Python dependencies (optional)
└── environment.yml           # Conda environment file (optional)

## Data Sources

https://d37ci6vzurychx.cloudfront.net/trip-data/yellow_tripdata_[2024-2014].[01-12]parquet


git clone https://github.com/rvasappa-ucsd/nyc-taxi-eda.git
cd nyc-taxi-eda

