# Greenness, Parks, and Mental Health in Washington, DC

**By:** Ashley Gyapomah

---

## Overview
This project investigates relationships between urban greenness, park exposure, and frequent mental distress across Washington, DC census tracts using spatial analysis, regression modeling, and machine learning.

Environmental greenness was quantified using satellite-derived NDVI data from Google Earth Engine alongside park polygon spatial data obtained from the DC Open Data Portal. These environmental variables were integrated with CDC PLACES mental health estimates and American Community Survey socioeconomic indicators.

Results demonstrated that poverty and unemployment were the strongest predictors of mental distress, while NDVI maintained a modest protective relationship after socioeconomic controls were introduced. Park-related variables did not independently predict mental distress once structural confounding factors were incorporated into the modeling framework.

## Research Question

Park-related variables did not independently predict mental distress once structural confounding factors were incorporated into the modeling framework.

## Repository Structure

project-folder/
│
├── data/
│   └── raw/
│
├── figures/
│
├── notebooks/
│   └── CapstoneProject.ipynb
│
├── report/
│   └── Greenness_Parks_and_Mental_Distress_DC.pdf
│
├── README.md
├── requirements.txt

## Datasets Used 
| Dataset | Purpose | Source |
| -------- | -------- | -------- |
| CDC PLACES | mental distress | CDC |
| NDVI | Environmetal Greenness | Google Earth Engine |
| ACS | Socioeconomic Control | Census API |
| Park Polygons | Park Exposure | DC Open Data |
| TIGER/Line | Census tract boundaries | U.S. Census |

## Data Access

Raw datasets are publicly available through the following sources:

- CDC PLACES
- Google Earth Engine
- U.S. Census ACS API
- DC Open Data Portal
- TIGER/Line Shapefiles

Due to file size limitations, raw spatial and satellite datasets are not stored directly within this repository.

## Methods Overview

The project integrated spatial analysis, feature engineering, exploratory data analysis, Ordinary Least Squares regression, validation analysis, and Random Forest modeling to evaluate relationships between environmental exposure and mental distress.

## Key Findings

- Poverty and unemployment were the strongest predictors of mental distress.
- NDVI retained a modest but statistically significant protective relationship.
- Park-related variables were not independently significant after socioeconomic controls were introduced.
- Results remained stable across multiple park exposure definitions and machine learning validation.

## Reproducibility

Install required packages:

```bash
pip install -r requirements.txt

