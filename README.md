# Berlin Air Quality Index (AQI) Analysis Dashboard

A comprehensive analysis of air quality patterns across Berlin's 12 districts, integrating hourly air quality data with meteorological variables to identify spatial and temporal trends in pollution levels.

## Overview

This project analyzes 3 years of hourly air quality and weather data (2023-2025) across all 12 Berlin boroughs (Bezirke). The analysis combines statistical modeling, geospatial analysis, and interactive visualization to understand how air quality varies by location and weather conditions.

## Features

- **Data Collection**: Automated hourly data retrieval from Open-Meteo API
  - Air quality indices (European AQI, PM2.5, PM10, NO₂, O₃, SO₂, CO, CO₂)
  - Weather variables (temperature, humidity, wind speed, pressure, cloud cover)

- **Geospatial Analysis**: Integration with Berlin district boundaries (GeoJSON)
  - Spatial interpolation of monitoring points
  - District-level aggregation and comparison

- **Statistical Testing**:
  - Pairwise comparisons between boroughs (Tukey's HSD, t-tests)
  - Bonferroni correction for multiple comparisons
  - Effect size calculations (Cohen's d)
  - Weather-controlled residual analysis

## Data Sources

- **Air Quality**: [Open-Meteo Air Quality API](https://open-meteo.com/en/docs/air-quality-api)
- **Weather**: [Open-Meteo Archive API](https://open-meteo.com/en/docs/archive-api)
- **Geospatial**: Berlin district boundaries (GeoJSON format)
