🚖 NYC Taxi Trip Data - Spark-Based Exploratory Data Analysis

This project performs exploratory data analysis (EDA) on the NYC Yellow Taxi dataset using PySpark within a Jupyter Notebook. The workflow involves downloading raw taxi trip data, preprocessing it, and generating insights about trip patterns, fare dynamics, and temporal distributions.

Approach and Methodology
We set up a Spark-based exploratory data analysis environment for the NYC Taxi dataset. The approach followed these key steps:

Environment Setup: Configured an optimized Spark session with appropriate memory allocations and performance parameters.
Data Loading: Loaded the NYC Taxi trip data in Parquet format, which offers better performance than CSV for Spark processing.
Feature Engineering: Created derived features including:

Temporal dimensions (hour, day, month, year)
Trip characteristics (duration, speed)
Financial metrics (tip percentage)
Categorical variables (time of day, weekend indicator)


Data Cleaning: Filtered out anomalies and extreme values to ensure data quality, removing records with unrealistic trip distances, fares, passenger counts, and speeds.
Exploratory Analysis: Conducted multi-dimensional analysis examining:

Temporal patterns (hourly, daily, weekday vs. weekend)
Financial patterns (fare and tip relationships)
Trip characteristics (distance, duration, speed)


Visualization: Created visualizations including:

Time series plots of trip metrics by hour
Distribution histograms of key variables
Correlation analysis between metrics
Comparative analysis (weekday vs. weekend)

