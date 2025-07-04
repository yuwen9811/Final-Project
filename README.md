# Final-Project
# Project Hypothesis

H₀ (Null Hypothesis): There is no significant change in the interannual variability, onset timing, or spatial distribution of rainfall during Ghana’s March–June rainy season from 2000 to 2020.

H₁ (Alternative Hypothesis): There are significant changes in one or more of the following during the 2000–2020 period:
- Annual total rainfall
- Timing of rainy season onset
- Spatial variability of rainfall
- Frequency of extreme rainfall events

# Data Source

We will use **CHIRPS v2.0 daily precipitation data**:  
*Climate Hazards Group InfraRed Precipitation with Station Data (CHIRPS)*  
Global daily GeoTIFFs (p05):  
[https://data.chc.ucsb.edu/products/CHIRPS-2.0/global_daily/tifs/p05/](https://data.chc.ucsb.edu/products/CHIRPS-2.0/global_daily/tifs/p05/)

# Analysis Plan Summary

We will subset CHIRPS daily rainfall data over Ghana from 2000 to 2020, focusing on the March–June rainy season. Using xarray, numpy, and matplotlib, we will calculate national mean rainfall, seasonal totals, onset timing (via 5-day rolling means), interannual variability (CV), and frequency of extreme rainfall days (>90th percentile). Visualizations will include time series trends, onset shifts, spatial variability maps, and extreme event counts to evaluate rainfall pattern changes across Ghana.

# Visualization Figures
- Figure 1:
  a) Daily Rainfall during Rainy Seasons – A time series showing daily rainfall over Ghana for each March–June season from 2000 to 2020, illustrating the strong seasonal cycle and year-to-year variability in rainfall patterns.
  b) Annual Mean Precipitation – A line plot showing the annual mean rainfall in millimeters per year from 2000 to 2020, with an added trendline to highlight potential long-term changes in average precipitation.
- Figure 2: Onset Timing of Rainy Season - A line plot of the first day of each year when 5-day rainfall exceeds a threshold, showing whether the onset of the rainy season has shifted earlier or later over time.
- Figure 3: Interannual Coefficient of Variation (CV) - A time series showing the relative variability of national mean rainfall (CV = std/mean), indicating how consistent rainfall has been from year to year.
- Figure 4: Spatial Standard Deviation Map of Rainfall - A heatmap showing the spatial variability (standard deviation) of total rainy season precipitation across Ghana, highlighting areas of greater fluctuation.
- Figure 5: Trend in Extreme Rainfall Days (>90th Percentile) - A time series showing the number of days per year with rainfall exceeding the 90th percentile, revealing possible increases in rainfall extremes.
