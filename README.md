
# ⚡ Forecasting Household Energy Usage
=========================

![Project Banner](https://via.placeholder.com/1000x250.png?text=Your+Project+Banner+Here)

---


## 📋 Executive Summary 
**To be added after Sprint 3**

- **Key Takeaways (so far):**  
  1. Energy demand has a cyclic pattern
  2. Linear Regression Model with Weather Dataset Features, is performing the best so far
  

---

## 🚀 Motivation

Growing electricity demand and climate change require smarter household energy monitoring. This project leverages machine learning and weather data to forecast power usage, reduce costs, and improve sustainability. I also have most been working on timeseries data at work, and would like to understand through this project topic the statistical and ML analysis of time series forecasting.

---

## 🧠 Project Overview

### Problem Area

With the increasing urgency around climate change and energy sustainability, improving residential energy efficiency is a critical focus. In many households, energy usage patterns are not monitored or optimized, leading to wastage, increased costs, and higher carbon footprints. Smart grids and energy-aware applications can help users understand and adjust their energy consumption habits—but only if they’re powered by meaningful insights derived from real-world data.

This project explores the problem of **inefficient household energy consumption**, aiming to uncover patterns, peak usage times, and potential areas for conservation.

**Stakeholders impacted include:**
- Homeowners seeking to reduce energy bills.
- Utility companies planning demand response strategies.
- Policy-makers designing energy incentives or rebates.
- Smart home system developers.

### Proposed Data Science Solution

This project applies exploratory data analysis (EDA), time series modeling, and machine learning to:
- **Understand** household energy consumption patterns across days, weeks, and seasons.
- **Predict** future energy usage at different times of day.
- **Detect anomalies** that may indicate wasteful or unusual consumption.
- **Recommend** actionable energy-saving insights based on consumption behaviors.

Potential deliverables may include:
- A predictive model for household energy usage.
- Visual dashboards summarizing usage trends and alerts.
- Scenario-based energy-saving recommendations.

### Impact of the Solution

This solution aims to:
- Empower individuals with personalized, data-driven energy insights.
- Support utility providers with demand forecasting and load balancing.
- Inform broader sustainability goals by contributing to more efficient energy use at the household level.
- Lay groundwork for future integration with smart home and IoT systems that automate energy optimization.

### Dataset Descriptions

The dataset used is the **UCI Individual Household Electric Power Consumption Data Set**. It contains over **2 million measurements** gathered from a single household in Sceaux,Paris, France between **December 2006 and November 2010**.

**Source:** UCI Machine Learning Repository  
**Link:** [https://archive.ics.uci.edu/ml/datasets/individual+household+electric+power+consumption](https://archive.ics.uci.edu/ml/datasets/individual+household+electric+power+consumption)

#### Key Characteristics:
- Data is collected in **1-minute intervals**, resulting in high granularity.
- The dataset is rich enough to enable time series modeling and seasonality detection.
- Missing values and noisy readings are present, requiring cleaning and preprocessing.

#### Data Dictionary

| Column Name              | Data Type | Description |
|--------------------------|-----------|-------------|
| **Date**                 | object    | Date in format dd/mm/yyyy |
| **Time**                 | object    | Time in format hh:mm:ss |
| **Global_active_power**  | float     | Total active power consumed in kilowatts (kW) |
| **Global_reactive_power**| float     | Total reactive power consumed in kilowatts (kW) |
| **Voltage**              | float     | Average voltage (in volts) |
| **Global_intensity**     | float     | Average current intensity (in amperes) |
| **Sub_metering_1**       | float     | Energy (in watt-hours) for kitchen appliances (dishwasher, oven, microwave) |
| **Sub_metering_2**       | float     | Energy (in watt-hours) for laundry appliances (washing machine, dryer, etc.) |
| **Sub_metering_3**       | float     | Energy (in watt-hours) for water heater and air conditioning 



The other dataset is imported from **OpenMeteo API**, the dataset is related to weather and solar features. It contains over **34,00 rows** illustrating weather metrics from Paris, France between **December 2006 and November 2010**.

#### Key Characteristics:
- Data is collected in **1-hour intervals**
- No missing values or noisy readings are present, requiring no cleaning and preprocessing.

#### Data Dictionary

| Column Name              | Type      | Unit   | Category | Description|
|--------------------------|-----------|--------|----------|------------|
| **temperature_2m**       | float64   | °C     | Weather  | Outdoor air temperature measured at 2 meters above ground |
| **relative_humidity_2m**  | float64  | %      | Weather      | Relative humidity of air at 2 meters above ground.                          |
| **dew_point_2m**          | float64  | °C     | Weather      | Dew point temperature at 2 meters above ground.                             |
| **apparent_temperature**  | float64  | °C     | Weather      | Feels-like temperature considering wind and humidity.                       |
| **surface_pressure**      | float64  | hPa    | Weather      | Atmospheric surface pressure.                                               |
| **cloudcover**            | float64  | %      | Weather      | Fraction of sky covered by clouds.                                          |
| **windspeed_10m**         | float64  | m/s    | Weather      | Wind speed measured at 10 meters above ground.                              |
| **windgusts_10m**         | float64  | m/s    | Weather      | Wind gusts measured at 10 meters above ground.                              |
| **winddirection_10m**     | float64  | °      | Weather      | Wind direction at 10 meters above ground.                                   |
| **shortwave_radiation**   | float64  | W/m²   | Solar        | Incoming shortwave solar radiation.                                         |
| **direct_radiation**      | float64  | W/m²   | Solar        | Direct beam solar radiation.                                                |
| **diffuse_radiation**     | float64  | W/m²   | Solar        | Diffuse (scattered) solar radiation.                                        |

---
## 🛠️ Methodology

High-level view of the process:

![Pipeline Diagram](https://via.placeholder.com/900x400.png?text=Data+Pipeline+Diagram)

1. **Data Processing**  
   - Data cleaning, handling missing values, normalization  
   - Feature engineering (weather, lag features, rolling averages)  

2. **Modeling**  
   - Classical ML models: Random Forest, XGBoost  
   - Deep learning models: LSTM, Transformer-based approaches  

3. **Prototyping & Deployment**  -In progress
   - Streamlit for interactive dashboards  
   - Joblib dumps for reproducible ML models  
   - Containerization (Docker) for portability  

---

---

## 🎯 Progress

✅ Data cleaning and preprocessing  
✅ Exploratory data analysis (EDA) with visualizations  
✅ Feature engineering with weather data  
🚧 Model experimentation (Regression, ARIMA,  XGBoost, LSTM)  
🚧 Deployment using Streamlit  
🔜 Cloud integration (AWS/GCP for scalable deployment)  

---

## 🎥 Demo- In progress

- 📊 **Data Visualizations**:  
  ![Data Visualization Example](https://via.placeholder.com/600x350.png?text=Insert+Graph+Here)

- 💻 **Interactive Demo** (e.g., Streamlit):  
  [Try the App](https://streamlit.io/) (replace with your deployed app link)  

- 🎬 **Short Video**:  
  Upload a walkthrough GIF or Loom/Youtube video link here.  

---


## 📂 Organization

```bash
├── data/               # Dataset links + processed data
├── model/              # Trained models (joblib/pickle)
├── notebooks/          # Jupyter/Colab notebooks
├── docs/               # Final reports & presentations
├── references/         # Research papers, tutorials
├── src/                # Source code (refactored scripts)
├── .gitignore          # Files to ignore in version control
├── conda.yml           # Environment dependencies
├── README.md           # Project landing page (this file)
└── LICENSE             # License file
