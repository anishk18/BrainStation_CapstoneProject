# BrainStation Data Science Capstone Project
------------------------------------------------------------------------------

## Forecasting Household Electricity Usage
=========================

### 🧠 Project Overview
**Problem Area**
With the increasing urgency around climate change and energy sustainability, improving residential energy efficiency is a critical focus. In many households, energy usage patterns are not monitored or optimized, leading to wastage, increased costs, and higher carbon footprints. Smart grids and energy-aware applications can help users understand and adjust their energy consumption habits—but only if they’re powered by meaningful insights derived from real-world data.

This project explores the problem of inefficient household energy consumption, aiming to uncover patterns, peak usage times, and potential areas for conservation.

Stakeholders impacted include:

Homeowners seeking to reduce energy bills.

Utility companies planning demand response strategies.

Policy-makers designing energy incentives or rebates.

Smart home system developers.

Proposed Data Science Solution
This project applies exploratory data analysis (EDA), time series modeling, and machine learning to:

Understand household energy consumption patterns across days, weeks, and seasons.

Predict future energy usage at different times of day.

Detect anomalies that may indicate wasteful or unusual consumption.

Recommend actionable energy-saving insights based on consumption behaviors.

Potential deliverables may include:

A predictive model for household energy usage.

Visual dashboards summarizing usage trends and alerts.

Scenario-based energy-saving recommendations.

Impact of the Solution
This solution aims to:

Empower individuals with personalized, data-driven energy insights.

Support utility providers with demand forecasting and load balancing.

Inform broader sustainability goals by contributing to more efficient energy use at the household level.

Lay groundwork for future integration with smart home and IoT systems that automate energy optimization.

Dataset Description
The dataset used is the UCI Individual Household Electric Power Consumption Data Set. It contains over 2 million measurements gathered from a single household in Sceaux, France between December 2006 and November 2010.

Source: UCI Machine Learning Repository
Link: https://archive.ics.uci.edu/ml/datasets/individual+household+electric+power+consumption

Key Characteristics:
Data is collected in 1-minute intervals, resulting in high granularity.

The dataset is rich enough to enable time series modeling and seasonality detection.

Missing values and noisy readings are present, requiring cleaning and preprocessing.

Data Dictionary
Column Name	Data Type	Description
Date	object	Date in format dd/mm/yyyy
Time	object	Time in format hh:mm:ss
Global_active_power	float	Total active power consumed in kilowatts (kW)
Global_reactive_power	float	Total reactive power consumed in kilowatts (kW)
Voltage	float	Average voltage (in volts)
Global_intensity	float	Average current intensity (in amperes)
Sub_metering_1	float	Energy (in watt-hours) for kitchen appliances (dishwasher, oven, microwave)
Sub_metering_2	float	Energy (in watt-hours) for laundry appliances (washing machine, dryer, etc.)
Sub_metering_3	float	Energy (in watt-hours) for water heater and air conditioning
Unmeasured energy	float	Derived feature: energy not captured by sub meters (optional for modeling)



### Demo

... Show your work:
...     Data visualizations
...     Interactive demo (e.g., `streamlit` app)
...     Short video of users trying out the solution


### Methodology

... High-level diagrams of entire process:
...     various data processing steps
...     various modelling directions
...     various prototyping directions


### Organization

#### Repository 

* `data` 
    - contains link to copy of the dataset (stored in a publicly accessible cloud storage)
    - saved copy of aggregated / processed data as long as those are not too large (> 10 MB)

* `model`
    - `joblib` dump of final model(s)

* `notebooks`
    - contains all final notebooks involved in the project

* `docs`
    - contains final report, presentations which summarize the project

* `references`
    - contains papers / tutorials used in the project

* `src`
    - Contains the project source code (refactored from the notebooks)

* `.gitignore`
    - Part of Git, includes files and folders to be ignored by Git version control

* `conda.yml`
    - Conda environment specification

* `README.md`
    - Project landing page (this page)

* `LICENSE`
    - Project license

#### Dataset

... Google Drive links to datasets and pickled models

### Credits & References

... Include any personal learning
