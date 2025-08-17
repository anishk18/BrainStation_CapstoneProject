

# Forecasting Household Energy Usage


# 🧠 Project Overview

## Problem Area

With the increasing urgency around climate change and energy sustainability, improving residential energy efficiency is a critical focus. In many households, energy usage patterns are not monitored or optimized, leading to wastage, increased costs, and higher carbon footprints. Smart grids and energy-aware applications can help users understand and adjust their energy consumption habits—but only if they’re powered by meaningful insights derived from real-world data.

This project explores the problem of **inefficient household energy consumption**, aiming to uncover patterns, peak usage times, and potential areas for conservation.

**Stakeholders impacted include:**
- Homeowners seeking to reduce energy bills.
- Utility companies planning demand response strategies.
- Policy-makers designing energy incentives or rebates.
- Smart home system developers.

## Proposed Data Science Solution

This project applies exploratory data analysis (EDA), time series modeling, and machine learning to:
- **Understand** household energy consumption patterns across days, weeks, and seasons.
- **Predict** future energy usage at different times of day.
- **Detect anomalies** that may indicate wasteful or unusual consumption.
- **Recommend** actionable energy-saving insights based on consumption behaviors.

Potential deliverables may include:
- A predictive model for household energy usage.
- Visual dashboards summarizing usage trends and alerts.
- Scenario-based energy-saving recommendations.

## Impact of the Solution

This solution aims to:
- Empower individuals with personalized, data-driven energy insights.
- Support utility providers with demand forecasting and load balancing.
- Inform broader sustainability goals by contributing to more efficient energy use at the household level.
- Lay groundwork for future integration with smart home and IoT systems that automate energy optimization.

## Dataset Descriptions

The dataset used is the **UCI Individual Household Electric Power Consumption Data Set**. It contains over **2 million measurements** gathered from a single household in Sceaux,Paris, France between **December 2006 and November 2010**.

**Source:** UCI Machine Learning Repository  
**Link:** [https://archive.ics.uci.edu/ml/datasets/individual+household+electric+power+consumption](https://archive.ics.uci.edu/ml/datasets/individual+household+electric+power+consumption)

### Key Characteristics:
- Data is collected in **1-minute intervals**, resulting in high granularity.
- The dataset is rich enough to enable time series modeling and seasonality detection.
- Missing values and noisy readings are present, requiring cleaning and preprocessing.

### Data Dictionary

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



The other dataset is imported from **OpenMeteo API**, the dataset is related to weather features. It contains over **34,00 rows** illustrating weather metrics from Paris, France between **December 2006 and November 2010**.

### Key Characteristics:
- Data is collected in **1-hour intervals**
- No missing values or noisy readings are present, requiring no cleaning and preprocessing.

### Data Dictionary

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

