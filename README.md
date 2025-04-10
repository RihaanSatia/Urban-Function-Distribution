# Analyzing the Effect of Urban Function Distribution on Overall Mobility Patterns

## 📌 Project Overview

This project investigates how the distribution of urban functions — such as points of interest (POIs) and workplace locations — influences human mobility within two major U.S. cities: **New York** and **Los Angeles**. By comparing these cities’ structural and transportation differences, we aim to uncover how urban form affects commute distances, accessibility, and transportation reliance.

## 🎯 Objectives

- Compare urban spatial structures and mobility patterns in NY and LA.
- Analyze the spatial distribution of POIs and workplaces using geospatial methods.
- Understand how urban design and transit availability affect commute behavior.
- Generate insights for urban planning and transportation policy.

## 🛠️ Tools & Technologies

- **Python**
  - `GeoPandas`, `Shapely` — for geospatial analysis
  - `Matplotlib` — for data visualization
- **ArcGIS** — for multivariate spatial clustering
- **Moran’s I** — index for spatial autocorrelation and clustering

## Datasets Used

- **OpenStreetMap POI Data** — spatial layout of urban functions
- **COVID19USFlows** (June 2019) — human mobility patterns
- **TIGER/Line Shapefiles** — geographic reference for census mapping
- **LEHD Origin-Destination Employment Statistics (LODES)** — home-workplace mapping
- **NYC MTA Turnstile Data** — subway usage (New York only)

## Key Findings

### Spatial Clustering (Moran's I)
| City        | Moran’s I | P-Value |
|-------------|-----------|---------|
| New York    | 0.469     | 0.001   |
| Los Angeles | 0.296     | 0.001   |

- **New York**: Dense POI clusters near downtown — transit-oriented and economically compact
- **Los Angeles**: More evenly distributed POIs — car-centric development and broader spatial reach

### Workplace Distribution
- **New York**: Centralized, promoting shorter commutes (1–2 miles)
- **Los Angeles**: Decentralized, longer commute distances (20+ miles)

### Travel Distances
- NY: Commute peaks around 1–2 miles  
- LA: Commute peaks beyond 20 miles

## Conclusions

- New York exhibits compact urban form and transit-based mobility.
- Los Angeles shows urban sprawl with car-reliant travel.
- Both cities display a shared short-commute trend influenced by workplace proximity.
- Urban planning should focus on:
  - Developing local hubs
  - Enhancing public transit
  - Minimizing long-distance travel needs

## Future Work

- Incorporate **network-based analysis** of transportation infrastructure.
- Integrate **machine learning models** for predictive urban flow analysis.
- Expand to include more cities and **longitudinal data** to track changes over time.
