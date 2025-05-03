🚖 NYC Taxi Data Exploratory Analysis
A comprehensive data analysis framework using Apache Spark and Jupyter Notebook for exploring and analyzing NYC Taxi trip data.

Project Overview
This repository contains a Spark-based exploratory data analysis of the NYC Yellow Taxi dataset. The analysis focuses on understanding trip patterns, fare structures, tipping behavior, and other insights from the taxi data.

Approach:

1. Environment Setup
  
2. Data Engineering

Data Ingestion Method: Parquet format for optimized performance
Feature Engineering: Created temporal, spatial, and financial derived features
Data Cleaning: Removed outliers and invalid records

3. Analysis Components

Temporal Analysis: Patterns by hour, day, month, and weekday vs. weekend
Financial Analysis: Fare structure and tipping behavior
Trip Characteristics: Distance, duration, and speed relationships
Geospatial Analysis: Pickup and dropoff location patterns

4. Visualization
Various visualizations to understand patterns in the data:

Trip distribution by hour
Fare amount relationships
Weekday vs. weekend comparisons
Correlation analysis


Few Important Questions on what we want to look for justification of EDA on this dataset:

Temporal Patterns

How do taxi trips vary by hour of the day, day of the week, and month of the year?
Is there a significant difference in taxi usage between weekdays and weekends?
How have overall taxi usage patterns changed year over year (pre and post-pandemic)?
What are the busiest hours for NYC taxis and how does this affect our understanding of urban mobility?

Financial Analysis

What factors influence fare amounts the most (distance, duration, time of day)?
How do tipping patterns vary throughout the day and week?
Is there a correlation between trip distance and tip percentage?
How do passenger counts affect fare amounts and tipping behavior?

Operational Insights

What is the average speed of taxis during different times of the day, and how does this reflect traffic conditions?
What is the distribution of trip distances, and what does this tell us about typical taxi usage?
Are there any seasonal patterns in trip duration or distance?
What percentage of trips fall into short, medium, and long-distance categories?

