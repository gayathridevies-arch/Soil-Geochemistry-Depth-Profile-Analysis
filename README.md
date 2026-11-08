# Soil Geochemistry Depth Profile Analysis

A Python script for generating, analyzing, and visualizing depth-dependent soil geochemical trends across different soil horizons.

## Overview
Soil chemical properties vary vertically due to weathering, leaching, and organic matter accumulation. In this project, I wrote a Python script to simulate a 30-sample soil dataset across multiple sites and depth horizons, applying Pandas for statistical aggregation and Seaborn for geochemical data visualization.

## Methodology & Workflow
* **Sampling Structure:** Modeled 30 samples distributed across 10 virtual sites (`Site_01` to `Site_10`) at three standard depth intervals: `0-15 cm`, `15-30 cm`, and `30-50 cm`.
* **Geochemical Variables:**
  * **pH:** Simulated using normal distributions that increase with depth (`5.8` at the surface to `6.8` in deeper layers) to reflect vertical weathering and leaching gradients.
  * **Organic Carbon (`Organic_Carbon_%`):** Modeled to decrease down the profile (`3.8%` down to `1.2%`) to capture surface organic matter accumulation.
  * **Cation Exchange Capacity (`CEC_meq100g`):** Programmatically modeled as a linear function of Organic Carbon (`OC * 7.5`) with added random noise to examine nutrient retention.
* **Data Processing & Export:** Cleaned, reordered, and exported the complete dataset to `soil_geochemistry_data.csv`. Used Pandas `groupby` and `agg` operations to compute mean, standard deviation, maximum, and minimum values per depth horizon, saving the final summary to `soil_geochemistry_summary_stats.csv`.

## Visualizations
* **Depth Profile Boxplots:** Generates a Seaborn boxplot illustrating the distribution and decrease of Organic Carbon across the three depth horizons.
* **Correlation Analysis (`OC vs. CEC`):** Plots an Ordinary Least Squares (`regplot`) trendline to examine the positive relationship between Organic Carbon percentages and Cation Exchange Capacity.

## Tech Stack
* **Language:** Python
* **Data Manipulation:** Pandas, NumPy
* **Visualization:** Seaborn, Matplotlib

