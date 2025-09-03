# London Mobility

Analysis of urban mobility patterns in London using Transport for London (TfL) journey data.

## Goal
To understand transport patterns in London in order to identify congestion trends, popular routes, and opportunities for more sustainable mobility.

## Dataset
- **TfL Journeys by Mode** (`tfl-journeys-type.csv`)  
  Contains monthly journey counts (in millions) across different transport modes, including bus, Underground, DLR, tram, Overground, cable car, and TfL Rail.  
  Coverage: 2011 - 2025.  

## Features
- Analysis of journey volumes across transport modes  
- Identification of long-term trends, seasonal variation, and the impact of major events  
- Visualisation of mobility patterns over time  

## Tools & Technologies
- Python (pandas, matplotlib)  
- Google Colab  
- Git & GitHub for version control  

## Data Cleaning Summary
Data cleaning was carried out in Python using pandas to prepare the dataset for analysis.  
The following steps were applied:  
1. **Converted date columns** (`period_beginning`, `period_ending`) to datetime format.  
2. **Renamed columns** to snake_case for easier use in Python.  
3. **Handled missing values** in journey counts by filling them with `0`.  
4. **Removed duplicates** to prevent double-counting.  
5. **Verified column data types** for consistency.  
6. **Exported a cleaned dataset** (`tfl-journeys-type-cleaned.csv`) for reproducible analysis.  

---

## Analysis & Findings

### 1. Trends Across All Modes
![Trends in London Journeys](plots/trends.png)  
Bus and Underground dominate journeys across London. All modes show a sharp decline in 2020 due to COVID-19 restrictions.  

### 2. Bus vs Underground
![Bus vs Underground](plots/bus_vs_underground.png)  
Both modes declined significantly in 2020, but bus journeys recovered more quickly than the Underground, suggesting greater resilience.  

### 3. Seasonality
![Seasonality](plots/seasonality.png)  
Journeys consistently dip in August (holiday period) and December (Christmas), with peaks in spring and autumn months.  

### 4. Event Impact
![Event Impact](plots/event_impact.png)  
The 2012 Olympics boosted Underground journeys temporarily, while COVID-19 caused an unprecedented collapse in 2020.  

---

## Conclusion 
- Bus and Underground journeys form the backbone of London’s transport system, showing clear seasonal variation.  
- Bus travel recovered faster than the Underground following COVID-19, suggesting it is more resilient to disruption.  
- Major events such as the 2012 Olympics increased demand temporarily, whereas COVID-19 caused the steepest decline on record.  

---

## Next Steps
- Extend the analysis by incorporating cycling and walking datasets to capture active travel.  
- Investigate the impact of major infrastructure projects (e.g., the Elizabeth Line).  
- Apply forecasting models to predict future mobility patterns.  
