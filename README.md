# Soil-Geochemistry-Depth-Profile-Analysis
## Project Overview
This project simulates, analyzes, and visualizes synthetic soil horizon data to explore foundational geochemical relationships. Built using Python, it demonstrates environmental data science workflows tailored for soil science and academic applications (such as IMSOGLO).

## Scientific Objectives & Methodology
- **Depth-Dependent Simulation:** Modeled 30 soil samples across three standard depth horizons (`0-15 cm`, `15-30 cm`, and `30-50 cm`) across 10 virtual sites.
- **Geochemical Parameters:** 
  - **pH:** Monitored across horizons to reflect typical weathering and leaching profiles.
  - **Organic Carbon (OC_%):** Decreases with depth due to organic accumulation in topsoil.
  - **Cation Exchange Capacity (CEC):** Programmatically modeled as a direct function of Organic Carbon to reflect nutrient retention mechanics.
- **Statistical Summarization:** Utilized Pandas `groupby` aggregations to calculate mean and standard deviation profiles per depth horizon.

## Visualizations
1. **Boxplot Analysis:** Visualizes the distribution of Organic Carbon across soil depth horizons with custom transparency and styling (`seaborn`).
2. **Correlation Analysis (Scatter & Regression):** Maps the relationship between Organic Carbon and Cation Exchange Capacity with a fitted regression trendline, illustrating nutrient retention drivers.

## Repository Structure
- `soil_geochemistry_analysis.ipynb`: The primary Google Colab notebook containing data generation, analysis, and plotting code.
- `soil_geochemistry_summary_stats.csv`: Exported summary statistics table grouped by depth horizon.

## Tech Stack
- **Python**
- **Pandas & NumPy** (Data generation and manipulation)
- **Seaborn & Matplotlib** (Statistical data visualization)
