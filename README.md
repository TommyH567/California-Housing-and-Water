# 📊 California Housing & Water Data Projects

This repository contains two data-driven visualization projects focusing on critical issues in California:
1. 🏠 **California Housing Analysis** – explores geographic and economic patterns in home prices.
2. 💧 **California Groundwater Trends** – visualizes groundwater levels to understand water resource challenges.

Both projects use Python for data cleaning (in Google Colab) and Tableau for interactive dashboards. Ideal for portfolio demonstration, public policy insights, or environmental planning analysis.

---

## 🏠 Project 1: California Housing Analysis

### 🔍 Objective
Explore spatial and economic trends in California’s housing market using real-world data from 1990s census block groups.

### 📂 Dataset
- **Source**: [California Housing Prices - Kaggle](https://www.kaggle.com/datasets/camnugent/california-housing-prices)
- **Format**: CSV
- **Key Features**:
  - `median_house_value`
  - `median_income`
  - `housing_median_age`
  - `latitude`, `longitude`
  - `ocean_proximity`

### 📊 Dashboards

#### 1. Median House Value by Location
- **Chart Type**: Geographic heat map
- **Insight**: Higher values cluster near major coastal cities like SF and LA.

#### 2. Income Distribution
- **Chart Type**: Histogram (binned `median_income`)
- **Insight**: Most neighborhoods fall into middle-income brackets, with a few very high-income areas.

#### 3. Income vs. House Value
- **Chart Type**: Scatter plot
- **Insight**: Strong positive correlation with a plateau due to capped values in the dataset.

#### 4. Ocean Proximity vs. House Value
- **Chart Type**: Bar chart
- **Insight**: Proximity to ocean or bay significantly increases house value.

---

## 💧 Project 2: California Groundwater Trends

### 🔍 Objective
Visualize and analyze groundwater levels to highlight areas of water depletion or long-term sustainability risks.

### 📂 Dataset
- **Source**: [Continuous Groundwater Level Measurements - Kaggle](https://www.kaggle.com/datasets/alifarahmandfar/continuous-groundwater-level-measurements-2023)
- **Files Used**:
  - `gwl-monthly.csv`
  - `gwl-daily.csv`
  - `gwl-stations.csv`
- **Key Variables**:
  - `MSMT_DATE`: Date of measurement
  - `STATION`: Unique well ID
  - `WLM_RPE`: Reference Point Elevation
  - `GSE_WSE`: Depth from ground surface to water
  - `WSE`: Water Surface Elevation

### 📊 Dashboards

#### 1. Groundwater Trends Over Time
- **Chart Type**: Line chart (MSMT_DATE vs. WLM_RPE)
- **Insight**: Identifies stations with long-term groundwater depletion trends.
- **Filter**: Top 10 stations by number of records (to ensure consistency).

#### 2. Groundwater Elevation vs. Surface Elevation
- **Chart Type**: Scatter plot (WSE or GSE_WSE vs. WLM_GSE)
- **Insight**: Highlights elevation differences and water access depths across regions.
