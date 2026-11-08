# Soil Geochemistry Depth Profile Analysis

A Python script for analyzing and visualizing depth-dependent geochemical trends across soil horizons.

## Overview
Soil chemical properties shift noticeably with depth due to organic matter accumulation, leaching, and weathering. In this self-directed project, I generated a 30-sample soil horizon dataset to practice statistical aggregation and multi-variable geochemical plotting in Python.

## Methodology & Parameters
* **Sampling Structure:** Modeled 30 samples distributed across 10 sampling sites at three standard depth intervals: 0–15 cm, 15–30 cm, and 30–50 cm.
* **Geochemical Variables:**
  * **pH:** Reflects vertical leaching and weathering gradients down the profile.
  * **Organic Carbon (`OC_%`):** Modeled to decrease with depth, capturing surface organic matter accumulation.
  * **Cation Exchange Capacity (`CEC`):** Modeled as a function of Organic Carbon to examine how organic matter drives nutrient-holding capacity.
* **Statistical Summary:** Grouped the dataset by depth horizon in **Pandas** to calculate mean and standard deviation values, exporting the results to `soil_geochemistry_summary_stats.csv`.

## Visualizations
* **Depth Profile Boxplots:** Plots the vertical distribution of Organic Carbon across the three soil horizons using **Seaborn**.
* **OC vs. CEC Regression:** Examines the correlation between Organic Carbon and Cation Exchange Capacity using an Ordinary Least Squares (OLS) trendline.

## Tools & Libraries
* **Language:** Python
* **Data Handling:** Pandas, NumPy
* **Visualization:** Seaborn, Matplotlib.




