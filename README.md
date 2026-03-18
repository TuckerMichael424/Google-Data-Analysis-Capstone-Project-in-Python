# Cyclistic Rider Data Analysis

## Overview

This project is a data analysis case study based on the fictional Cyclistic bike rental company. The goal is to analyze data from Cyclistic's bike-sharing service and uncover insights related to user behavior. The analysis covers the period from April 2024 to March 2025, leveraging real-world data sourced from the Divvy Trip data for the same timeframe.

The analysis was conducted as part of the Google Data Analytics Professional Certificate Capstone Project, with the dataset processed and analyzed using Python. The primary objective is to provide actionable insights for Cyclistic's marketing and management teams to make data-driven decisions that improve customer engagement and operational efficiency.

## Objective

The main objectives of this case study are:
- Understand the key metrics of riders using Cyclistic's rental bikes, including:
  - Types of users (Casual vs. Members)
  - Types of rideables (e.g., classic bikes, electric bikes, electric scooters)
  - Temporal usage patterns (times of day, days of the week, months, and seasons)
  - Most frequent stations for bike starts and ends.
- Provide actionable marketing and operational recommendations based on data insights.

## Data Source

This project uses the following dataset:

- **Divvy Trip Data** (2024-2025) - Dataset provided by Motivate International Inc. under the MIT License.
- The dataset contains information about the rides, including:
  - `ride_id`: A unique identifier for each ride
  - `rideable_type`: Type of bike or scooter used
  - `started_at` & `ended_at`: Timestamp for when the ride started and ended
  - `start_station_name` & `end_station_name`: Station names for the starting and ending points
  - `start_station_id` & `end_station_id`: Unique identifiers for the stations
  - `member_casual`: Type of rider (member or casual)

## Methodology

### 1. Data Cleaning & Preparation
- **Null Values**: Any rows with missing data were removed, particularly for station names.
- **Data Types**: The `started_at` and `ended_at` columns were converted to the appropriate datetime format.
- **Outliers**: Negative or zero ride durations were removed. Very long ride durations were capped for visualization purposes.

### 2. Exploratory Data Analysis (EDA)
The following key metrics were analyzed:
- **Rider Types**: Membership (member vs. casual) and their impact on ride duration and frequency.
- **Rideable Types**: Comparison of classic bikes, electric bikes, and electric scooters.
- **Temporal Usage Patterns**: Analyzed the distribution of rides by hour, day, week, month, and season.
- **Station Usage**: Identified the most popular start and end stations.
- **Ride Duration**: Investigated ride durations across various rider and rideable types.

### 3. Data Visualization
Several visualizations were created, including:
- Bar charts for the distribution of rider types and rideable types.
- Histograms and boxplots for ride durations.
- Time series plots for ride volumes across different hours of the day, days of the week, and months of the year.
- Heatmaps for the usage of start and end stations.

### 4. Recommendations
Based on the findings, the following recommendations were made:
- **Marketing Campaigns**: Focus on casual riders, especially over weekends. Promotional material should target high-traffic stations.
- **Product Strategy**: Classic bikes dominate ridership and should be promoted as the primary offering.
- **Station Focus**: The top stations should be the focus of advertising and bike placement for maximum exposure.

## Steps Taken in the Analysis

1. **Data Import & Initial Exploration**: Importing the data and performing initial checks, including null value handling and duplicate removal.
2. **Data Transformation**: Standardized the data types for datetime fields and created new features (e.g., ride duration, time of day, day of the week, month, season).
3. **Exploratory Analysis**: Grouped data by different categories to analyze key metrics and identify trends.
4. **Visualizations**: Created various plots to help stakeholders understand the trends and insights from the data.
5. **Conclusions & Recommendations**: Provided actionable insights based on the analysis, including marketing and operational suggestions.

## Files in This Repository

- `cyclistic_rider_data_analysis.py`: The main script for the analysis, including all data cleaning, transformation, and visualization steps.
- `Cyclistic_Rider_Analysis_Report.md`: A comprehensive markdown file with detailed results and recommendations based on the analysis.
- `cyclistic-rider-case-study-python.ipynb`: Jupyter notebook with the entire project workflow, including code and visualizations.

## How to Run

To run the analysis, follow these steps:

1. Clone this repository to your local machine.
2. Install the necessary Python packages by running:

   ```bash
   pip install -r requirements.txt
