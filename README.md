# Saudi Cities Walk Score
#### Purpose: Misk Academy Data Science Immersive Bootcamp 2021 Capstone Project
#### Author: Laian Abussaud
#### Instructor: Rick Scavetta
#### Teaching Assistant: Lujain Felemban
#### Date: Novemeber 16th, 2021

## Contents
1. Overview
2. Objectives
3. Research Questions
4. Notebooks Description
5. Dataset Description
6. Notes

## Overview
This project aims to understand the Saudi urban conditions better by addressing the walkaing conditions in Saudi cities. The choosen 4 Saudi cities are (Riyadh, Jeddah, Mecca, Al Khobar).

## Objectives
- To analyze and visualize Saudi cities walkability conditions
- To provide a comprehensive dataset containing all necessary data
- To create a walk score measure index that is suitable for the Saudi context

## Research Questions
- Are Saudi cities walkable? Can most daily errands be completed on foot?
- Which Saudi city in the analysis is the most walkable?
- What features are important to build a Saudi city walk score?

## Notebooks Descriptions
1. **Data_Collection**
2. **Data_Preperation**
3. **EDA** (Exploratory Data Analysis)
4. **ML_Modeling** (Machine Learning Modeling)
5. **Saudi Walk Score**

## Dataset Description
The analysis was done with a custom data set by collecting a diverse set of cities data and multiple API sources to train a machine learning model to predict the walk score.

Data sources:
- **Walk Score API:** returns a walk score, transit score and bike score for any location. (only used walk score)
- **OSMnx:** Python package that lets you download spatial geometries and model, project, visualize, and analyze street networks from OpenStreetMap’s APIs.
- **Google Places API:** returns information about places. Places are defined within this API as establishments, geographic locations, or prominent points of interest.
- **Google Reverse Geocoding API:** reverse geocoding is the process of converting geographic coordinates into a human-readable address.
- **OpenWeather API:** returns the current weather conditions for a geolocation.
- **LocationIQ:** Nearby Points of Interest (PoI) API returns specified PoIs or places around a given coordinate.

Data categories:
- Geolocations:
  - Latitude
  - Logitude
  - City

- Amenity-based:
  - Walk score
  - Amenities (all within 1000m radius)
    - Supermarket count
    - School count
    - Hospital count
    - Clinic count
    - Pharmacy count
    - Restaurant count
    - Cafe count
    - Park count

- Census-based:
  - Zoning category
  - Population
  - Population density

- Weather-based:
  - Temperature
  - Temperature time stamp
  - Temperature week day
  - UV index

- City Street Network Structure:
  - Intersection count
  - Street per node average
  - Circuity average
  - Street lenght average

- Distance-based:
  - Closest highway
  - Closest primary road
  - Closest secondary road
  - Closest residentail road
  - Closest commercial zone

| **Features** | **Description** |
| :---: | :---: |
| lat  | latitude: measurement of distance north or south of the Equator |
| lon | longitude: measurement of distance east or west of the Equator |
| point | (latitude, longitude) |
| city | point corresponding city |
| walk_score | from WalkScore API https://www.walkscore.com/professional/api.php |
| amenities_count | different amenities count from OpenStreetMap (OSM) API https://www.openstreetmap.org/#map=5/25.245/43.088 |
| zip_code | zoning category |
| pop | city's population |
| pop_density | city's population density |
| temp | city's temperature |
| time_stamp | temperature time stamp |
| week_day | temperature week day  |
| uv_index | UV index |

## Notes
This project is a work in progress as I add more relevant data to the dataset and become a better spatial data scientist
