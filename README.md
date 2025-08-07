California Housing & Water Data Projects

This README contains two data-driven visualization projects focusing on critical issues in California:
1. California Housing Analysis – explores geographic and economic patterns in home prices.
2. California Groundwater Trends – visualizes groundwater levels to understand water resource challenges.

Both projects use Python for data cleaning (in Google Colab) and Tableau for interactive dashboards. 

---

Project 1: California Housing Analysis

Objective:
Explore spatial and economic trends in California’s housing market using real-world data from 1990s census block groups.

Dataset
- Source: [California Housing Prices - Kaggle](https://www.kaggle.com/datasets/camnugent/california-housing-prices)
- Format: CSV
- Key Features:
  - median_house_value
  - median_income
  - housing_median_age
  - latitude and longitude
  - ocean_proximity

Dashboards

1. Median House Value by Location
- Chart Type: Geographic heat map
- Insights: Higher values are near major cities like San Francisco and Los Angeles.

2. Income Distribution
- Chart Type: Histogram (binned by `median_income`)
- Insights: Most households fall into low-to-middle income brackets, with a few in the very high-income bins.

3. Income vs. House Value
- Chart Type: Scatter plot
- Insights: Strong positive correlation with a plateau due to capped values in the dataset.

4. Ocean Proximity vs. House Value
- Chart Type: Bar chart
- Insights: Proximity to ocean or bay significantly increases house value.

Overall Findings: -----

---

Project 2: California Groundwater Trends

Objective
Visualize and analyze groundwater levels to highlight areas of water depletion or long-term sustainability risks.

Dataset
- Source: [Continuous Groundwater Level Measurements - Kaggle](https://www.kaggle.com/datasets/alifarahmandfar/continuous-groundwater-level-measurements-2023)
- Files Used:
  - `gwl-monthly.csv`
  - `gwl-daily.csv`
  - `gwl-stations.csv`
- Key Variables:
  - `MSMT_DATE`: Date of measurement
  - `STATION`: Unique well ID
  - `WLM_RPE`: Reference Point Elevation
  - `GSE_WSE`: Depth from ground surface to water
  - `WSE`: Water Surface Elevation

Dashboards

1. Groundwater Trends Over Time
- Chart Type: Line chart (MSMT_DATE vs. WLM_RPE)
- Insight: Identifies stations with long-term groundwater depletion trends.
- Filter: Top 10 stations by # of records (to ensure consistency).

2. Water Surface Elevation quality by station
- Chart Type: Scatter plot (WSE vs. # of records)
- Insight: Highlights which wells/area of wells has the more confidence in wse measurements.
- Filter: Top 10 stations by # of records


Overall  Findings: The first line chart gave me the information that the wells with the higher water level measurement reference point elevation are in areas more north, closer to Sacramento. Whereas, the wells with the lower reference point elevation are more towards San Francisco/San Jose. These insights are useful because they can tell us a lot about the water flow patterns in these areas. The second chart shows which wells have a more confident water surface elevation measurement. So we can see that most wells have a high confidence in wse measurements, but my main takeaway from this is that a majority of the wells without a confident wse measurement are in stations in Northern California (Near Sacramento). This can tell us that the measurements on the water surface elevation are much more accurate in certain areas compared to other areas, which could help ensure more accurate research on water flow and water supply in California.
