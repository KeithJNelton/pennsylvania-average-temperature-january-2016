## Overview
This project visualizes average January 2016 temperatures across Pennsylvania using NOAA daily station data. Thirteen station readings were cleaned and interpolated in QGIS to produce a temperature choropleth clipped to the state boundary.

![Map](Average%20Temperature%20Pennsylvania%20(January%202016).png)

## Purpose
I completed this project to gain hands-on experience using QGIS and revisit basic statistical analysis learned during undergraduate coursework. Further, the project leaves room for future inquiry into weather patterns across Pennsylvania, such as changes in temperature trends or correlations between rising temperatures and precipitation. 

## Workflow
1. Compiled NOAA station CSVs into a master dataset
2. Filtered to January 2016 and averaged temperature per station (LibreOffice Calc pivot tables)
3. Converted temperature values from tenths of °C to °F
4. Cleaned erroneous records (station ID prefixes pulling in South American stations, for some reason)
5. Joined station coordinates back to the temperature data
6. Imported points into QGIS, reprojected to EPSG:5070
7. Generated an interpolated surface using IDW Interpolation, clipped to the Pennsylvania state boundary
8. Styled and exported the final choropleth-style map
