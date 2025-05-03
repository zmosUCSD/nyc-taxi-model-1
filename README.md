# 🚖 NYC Taxi Data Exploratory Analysis

A comprehensive data analysis framework using **Apache Spark** and **Jupyter Notebook** for exploring and analyzing NYC Yellow Taxi trip data.

---

## 📌 Project Overview

This repository provides a Spark-based exploratory data analysis of the NYC Yellow Taxi dataset. The analysis focuses on understanding:

- Trip patterns
- Fare structures
- Tipping behavior
- Operational trends
- Urban mobility insights

---

## ⚙️ Approach

### 1. Environment Setup

Set up Spark and Jupyter environment either locally or on a distributed cluster (e.g., AWS EMR, Databricks).

### 2. Data Engineering

- **Data Ingestion**: Downloaded Parquet-format Yellow Taxi trip data for high-speed Spark loading.
- **Feature Engineering**:
  - Extracted **temporal features** (hour, day, month)
  - Derived **trip metrics** (speed, duration, tip %)
- **Data Cleaning**:
  - Removed invalid entries (e.g., zero distance, negative fare)
  - Filtered outliers using domain-driven thresholds

### 3. Analysis Components

#### 📅 Temporal Analysis
- Trip volume by hour of day, day of week, and month
- Weekday vs. weekend usage comparison
- Year-over-year trends (including pre- vs. post-pandemic analysis)

#### 💰 Financial Analysis
- Fare vs. distance/time relationship
- Tip behavior patterns
- Tip % distribution and influencing factors

#### 🚕 Trip Characteristics
- Distribution of distance and duration
- Speed patterns by time of day
- Categorization of trips by distance: short, medium, long

#### 🗺️ Geospatial Patterns *(Planned/Optional)*
- Pickup and dropoff location clustering
- High-density zones (e.g., airports, entertainment districts)

### 4. 📊 Visualization Highlights

- Trip distribution by hour and day
- Fare amount vs. distance scatter plots
- Tip % by time window
- Weekday vs. weekend comparisons
- Correlation heatmaps for key metrics

---

## ❓ Key Exploratory Questions

### 📅 Temporal Patterns
- How do taxi trips vary by hour, day, and month?
- Is weekday usage significantly different from weekends?
- How have trip patterns changed pre- vs. post-COVID?
- What are the busiest times for NYC taxis?

### 💸 Financial Insights
- Which factors (e.g., distance, time) drive fare amounts?
- Do tipping patterns vary by time of day or weekday?
- Is there a link between trip length and tipping percentage?
- How does passenger count influence fare and tips?

### 🧭 Operational Insights
- What is the average taxi speed by hour — how does this reflect traffic?
- What does the trip distance distribution reveal about travel behavior?
- Are there seasonal trends in trip duration?
- How many trips fall into short (0–2 mi), medium (2–10 mi), and long (>10 mi) categories?

---

## 📂 Repository Structure

<pre> nyc-taxi-eda/ ├── nyc_taxi_eda.ipynb # Main Jupyter Notebook for Spark-based EDA ├── nyc_taxi_data/ # Folder to store downloaded Parquet files ├── README.md # Project overview and documentation ├── requirements.txt # Python dependencies (optional) └── environment.yml # Conda environment file (optional) </pre>

---

## 📎 Data Source

NYC Taxi and Limousine Commission (TLC):  
🔗 [https://www.nyc.gov/site/tlc/about/tlc-trip-record-data.page](https://www.nyc.gov/site/tlc/about/tlc-trip-record-data.page)

Parquet files used:  
🔗 `yellow_tripdata_2022-01.parquet`, `yellow_tripdata_2022-02.parquet`, `yellow_tripdata_2022-03.parquet`

---

## 🚀 Getting Started

1. Clone this repo  
   ```bash
   git clone https://github.com/rvasappa-ucsd/nyc-taxi-eda.git
   cd nyc-taxi-eda
2. Launch Jupyter Notebook in SDSC Portal and run nyc_taxi_eda.ipynb


