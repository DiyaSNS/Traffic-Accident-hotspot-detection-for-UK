
# Geospatial Predictive Modelling of Road Accident Hotspots
Using UK Stats19 Collision Data & Spatial Machine Learning

📌 1. Project Overview

Road accidents are not random — they cluster in specific locations due to road layout, traffic exposure, and environmental conditions.
This project builds a complete geospatial predictive modelling pipeline that identifies and forecasts accident hotspots across the UK using:

503,000+ police-reported collision records (Stats19)

5.5 million road segments from OpenStreetMap

Spatial grid modelling

Machine learning (Random Forest)

The goal is to answer:

Which areas are structurally prone to road accidents, and can we predict future hotspot intensity using spatial features?

This project mirrors real-world workflows used in:

Transportation planning

Urban safety analysis

Predictive policing

Intelligent mobility systems

🗂️ 2. Data Sources
🟦 Stats19 UK Police Collision Data (2019–2024)

Includes:

Latitude / longitude

Accident severity

Road & weather conditions

Police force

Number of vehicles

Road environment

🟩 OpenStreetMap Road Network

Downloaded in 142 spatial chunks to avoid API limits and memory issues.

Contains:

Road geometry

OSM highway type

Multi-lane information

Intersection nodes

🧩 3. Methodology

This project uses a grid-based spatial modelling approach, a standard method in geospatial predictive analytics.

✔ Step 1 — Accident Data Cleaning

✔ Step 2 — Create a Nationwide Spatial Grid

✔ Step 3 — OSM Road Network Extraction (142 Chunks)

✔ Step 4 — Feature Engineering

✔ Step 5 — Train Predictive ML Model

✔ Step 6 — Spatial Cross-Validation

✔ Step 7 — Hyperparameter Tuning

📊 4. Model Performance
Metric	Score
R²	0.93

RMSE	≈ 15 accidents per grid

Feature Importances	Road length (79%)

Intersection count (21%)

This is outstanding performance for national-scale geospatial modelling.

🗺️ 5. Outputs & Visualizations

🔥 Accident Hotspot Map
Predicted intensity per grid cell (choropleth)

🛣 Road Network Density Map

✳ Intersections Density Map

💡 SHAP Explanations
