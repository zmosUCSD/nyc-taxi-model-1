# 🚖 NYC Taxi Data Exploratory Analysis

A comprehensive data analysis framework using **Apache Spark** and **Jupyter Notebook** for exploring and analyzing NYC Yellow Taxi trip data from 2014 through 2024.

---

## 📌 Project Overview

This repository provides a Spark-based exploratory data analysis (EDA) of the NYC Yellow Taxi dataset. The analysis focuses on understanding:

- Trip patterns
- Fare structures
- Tipping behavior
- Operational trends
- Urban mobility insights over the past decade

---

## ⚙️ Approach

### 1. Environment Setup

- Apache Spark and PySpark configured within a Jupyter Notebook environment
- Compatible with both local and distributed deployments (e.g., Databricks, AWS EMR)

### 2. Data Engineering

- **Data Ingestion**: NYC Yellow Taxi trip data (2014–2024, all months) in Parquet format
- **Feature Engineering**:
  - Temporal features (hour, day, month, weekday/weekend)
  - Trip metrics like speed, duration, tip percentage
- **Data Cleaning**:
  - Removal of invalid trips (e.g., 0 distance/fare)
  - Filtering outliers and noisy records

### 3. Analysis Components

#### 📅 Temporal Analysis
- Hourly, daily, and monthly trip trends
- Year-over-year change tracking
- Weekday vs. weekend usage patterns

#### 💰 Financial Analysis
- Fare vs. trip distance/time correlation
- Tipping trends and tip percentage distribution
- Fare dynamics based on passenger count and trip type

#### 🚕 Trip Characteristics
- Trip speed analysis by hour
- Distance/duration categorization (short, medium, long)
- Temporal effects on trip length

#### 🗺️ Geospatial Analysis *(Planned/Future Work)*
- Pickup/dropoff clustering
- High-density zones and airport corridors

---

## 📊 Visualization Highlights

- Hourly and weekly trip distribution
- Fare vs. distance scatter plots
- Tip percentage histograms and time-of-day analysis
- Correlation heatmaps of trip features

---

## ❓ Key Exploratory Questions

### Temporal Patterns
- How do taxi usage patterns vary across time of day, day of week, and year?
- What are the busiest hours for NYC taxis?
- How has usage changed post-COVID compared to pre-pandemic years?

### Financial Insights
- What are the strongest predictors of fare amount?
- When are riders more likely to tip?
- Do trip distance and passenger count influence tips?

### Operational Insights
- What’s the average taxi speed across different times?
- How do trip durations and distances vary seasonally?
- What share of rides are short (<2 mi), medium (2–10 mi), and long (>10 mi)?

---

## 📂 Repository Structure

```text
nyc-taxi-eda/
├── nyc_taxi_eda.ipynb        # Main Jupyter Notebook for Spark-based EDA
├── nyc_taxi_data/            # Folder for downloaded Parquet trip data
├── README.md                 # Project overview and documentation
├── requirements.txt          # Python dependencies (optional)
└── environment.yml           # Conda environment file (optional)
```

---

## 📎 Data Source

This project uses publicly available NYC Yellow Taxi data published by the NYC Taxi & Limousine Commission (TLC).

- **Official TLC page**:  
  https://www.nyc.gov/site/tlc/about/tlc-trip-record-data.page

- **Parquet file archive (2014–2024)**:  
  All monthly files accessed via CloudFront CDN:  
  ```
  https://d37ci6vzurychx.cloudfront.net/trip-data/yellow_tripdata_[2014-2024].[01-12].parquet
  ```

- **File Format**: Parquet (columnar, efficient for Spark)

---

## 🚀 Getting Started

### 1. Clone the Repository

```bash
git clone https://github.com/rvasappa-ucsd/nyc-taxi-eda.git
cd nyc-taxi-eda
```

### 2. Set Up the Environment

Using Conda:

```bash
conda env create -f environment.yml
conda activate nyc-taxi-eda
```

Using pip:

```bash
pip install -r requirements.txt
```

### 3. Launch the Notebook

```bash
jupyter notebook
# Open nyc_taxi_eda.ipynb and run cells
```

---

## 📈 Future Enhancements

- Interactive dashboard using Plotly Dash or Streamlit
- Advanced geospatial analysis using H3 or GeoPandas
- Expand to green/bike/for-hire vehicle datasets

---

## 👩‍💻 Authors

This project is developed by students at **UC San Diego** as part of 232-R Group Project Spring Semester:

- **Harsh Arya** — harya@ucsd.edu  
- **Gabrielle Despaigne** — gdespaigne@ucsd.edu  
- **Zack Mosley** — zmosley@ucsd.edu  
- **Camila Paik** — capaik@ucsd.edu  
- **Raghav Vasappanavara** — rvasappanavara@ucsd.edu

---

## 📄 License

This repository is for educational and research purposes. Data is publicly available and governed by NYC TLC data usage policies.

---
