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
This project aims to understand the Saudi urban conditions better by addressing the walkabilty conditions in Saudi cities. The choosen 4 Saudi cities are (Riyadh, Jeddah, Mecca, Al Khobar).

## Objectives
- To analyze and visualize Saudi cities walkability conditions
- To provide a comprehensive dataset containing all necessary data
- To create a walk score measure that is suitable for the Saudi context

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
The analysis was done on an aggregated dataset from different sources.
Data sources:
- **Walk Score API:** returns a walk score, transit score and bike score for any location.
- **Google Elevation API:** returns elevation data for all locations on the surface of the earth.
- **Google Places API:** returns information about places. Places are defined within this API as establishments, geographic locations, or prominent points of interest.
- **Google Reverse Geocoding API:** reverse geocoding is the process of converting geographic coordinates into a human-readable address.
- **Weather Company Data:** returns the current weather conditions for a geolocation.
- **LocationIQ:** Nearby Points of Interest (PoI) API returns specified PoIs or places around a given coordinate.
- **OSMnx:** Python package that lets you download spatial geometries and model, project, visualize, and analyze street networks from OpenStreetMap’s APIs.

- Seattle City Zoning: Zoning districts specify a category of use (e.g., single-family residential, multifamily residential, commercial, industrial, etc.)
- Seattle Census Data: Provides population and area in square miles for census tracts within Census Tracts and Geographic Identifiers
- U.S. Census Geocoder API: For a given geolocation, the API returns Census tracts and unique Geographic Identifiers. This was crucial for correctly merging in Zoning and Census data.

- Coordinates (latitude, longitude) of different Saudi cities
- OSM data
- WalkScore API's
- Pedestrian First API's
- Weather API's

The dataset contains the following features:
| **Features** | **Description** |
| :---: | :---: |
| Name | Point name |
| City | Name of the city |
| Latitude  | Measurement of distance north or south of the Equator |
| Longitude | Measurement of distance east or west of the Equator |
| WalkScore | WalkScore API from |
| Pedestrian First | Pedestrian First API from |
| Weather | Weater API from |

You can access the dataset directly from the data folder in this repository.

## Notes
This project is a work in progress as I add more relevant data to the dataset and become a better spatial data scientist
