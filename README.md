# Household Power Consumption Analysis

Exploratory data analysis (EDA) on 2 years of minute-by-minute 
household electricity consumption data (2006-2008), uncovering 
seasonal patterns, peak usage hours, and anomalies.

## Dataset
- 1,048,575 rows of minute-by-minute electricity readings
- Period: December 2006 — December 2008
- Source: `household_power_consumption.csv`

## Project Workflow
CSV Data → Python (EDA & Visualization) → Power BI (Dashboard)

## Analysis & Key Findings

### 📈 Monthly Consumption Trend
- Clear seasonal pattern across 2 years
- Suspicious drop around September 2008 — likely household absence

### 🌡️ Seasonal Pattern
- **December** has the highest consumption (~1.65 kW)
- **August** has the lowest consumption (~0.53 kW)
- U-shaped pattern — high in winter, low in summer, rising in autumn

### ⏰ Peak Usage Hours
- **Morning peak: 7-8 AM** (~1.5 kW) — morning routine
- **Evening peak: 7-9 PM** (~2.0 kW) — highest usage of the day
- **Lowest usage: 2-4 AM** (~0.45 kW) — household asleep

### 🔴 Anomaly Detection (3-Sigma Rule)
- 18,000+ anomalies detected out of 1M readings
- Spikes reaching up to 10-11 kW
- Gaps in data confirm periods of household absence

### ⚡ Sub Metering Comparison
- **Sub_metering_3** (water heater/AC) dominates energy usage
- **Sub_metering_1 & 2** (kitchen & laundry) remain consistently low
- Sub_metering_3 dips in summer — less heating required

## Tools Used
- Python (Pandas, Matplotlib, Seaborn)
- Power BI Desktop
- Jupyter Notebook