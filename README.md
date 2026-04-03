# Cascade Snow Water Equivalent Analysis: 1992–2022 🏔️❄️
Exploratory Data Analysis on Snow Water Equivalent (SWE) Trends in the Cascade Range from 1992 - 2022

## 📋 Project Overview
This report investigates daily SWE measurements at two key SNOTEL locations—**Hogg Pass** and **Santiam Junction**—over a 30-year period. The analysis is shifted from calendar years to **Water Years** (Oct 1 – Sep 30) to provide a more accurate representation of annual snowpack accumulation and melt cycles.

## 📊 Key Insights

### 1. Decadal Decline in Peak Snowpack
The analysis reveals a **general decline in the yearly peak amount of snow** at both stations from 1992 to 2022.  
* **Hogg Pass:** Absolute peak SWE dropped from a high of 68.5 (1998) to below 3.0 (2014). While the data fluctuates, every major peak following 1998 has been lower than the one preceding it.
* **Santiam Junction:** Follows a similar downward trajectory, with recent peaks failing to reach the historical highs of the late 1990s and early 2000s.

### 2. Station Comparison (2018 Water Year)
A deep dive into the 2018 water year highlights significant elevational or locational differences:
* **Higher Yield:** Hogg Pass consistently recorded higher daily SWE values than Santiam Junction throughout the entire season.
* **Duration:** The analysis identifies the specific "First Nonzero" and "Last Nonzero" SWE dates, defining the exact window of the snow season for both locations.

## 🛠️ Technical Stack
* **Language:** R
* **Libraries:** `tidyverse`, `dplyr`, `readr`, `lubridate`, `knitr`
* **Data Source:** USDA Natural Resources Conservation Service (NRCS)

## 📂 Data Processing Highlights
* **Water Year Transformation:** Reassigned October–December dates to the following year's water cycle.
* **Tidy Data:** Converted wide-format monthly SNOTEL reports into a long-format time series for ggplot2 visualization.
* **Peak Detection:** Grouped operations to extract the `max_SWE` per station per year.

## 🚀 Usage
1. Clone the repo.
2. Ensure the SNOTEL data is located at `data/report.csv`.
3. Render the analysis
---
**Author:** Aren Lampman 

