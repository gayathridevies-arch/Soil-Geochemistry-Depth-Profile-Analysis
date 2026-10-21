# Soil-Geochemistry-Depth-Profile-Analysis
A Python pipeline for analyzing and visualizing synthetic soil horizon data to explore depth-dependent geochemical trends. Developed to support environmental data analysis workflows and academic preparation (such as IMSOGLO).

## Overview
This script generates and evaluates a 30-sample synthetic soil dataset to examine how key chemical properties vary across soil profiles. It handles data simulation, statistical aggregation, and multi-variable plotting using standard data science libraries.

## Methodology & Parameters
- **Sampling Design:** Modeled 30 samples across three standard depth horizons (0–15 cm, 15–30 cm, and 30–50 cm) across 10 virtual sites.
- **Geochemical Variables:**
  - **pH:** Tracks weathering and leaching gradients with depth.
  - **Organic Carbon (OC_%):** Decreases down the profile to reflect surface organic accumulation.
  - **Cation Exchange Capacity (CEC):** Programmatically modeled as a function of Organic Carbon to simulate nutrient retention mechanics.
- **Aggregation:** Uses Pandas groupby operations to compute mean and standard deviation profiles per depth horizon, exported to `soil_geochemistry_summary_stats.csv`.

## Visualizations
1. **Depth Profile Boxplots:** Visualizes the distribution of Organic Carbon across soil horizons using Seaborn.
2. **Correlation Analysis:** Maps the relationship between Organic Carbon and Cation Exchange Capacity with an OLS regression trendline.

## Tech Stack
- **Language:** Python
- **Data Manipulation:** Pandas, NumPy
- **Visualization:** Seaborn, Matplotlib


