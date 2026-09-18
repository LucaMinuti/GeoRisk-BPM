# GeoRisk

**Building-level landslide and flood risk scoring for the Italian insurance market.**

GeoRisk turns a building's address into a risk score (0–100) for landslide and flood hazard in a few seconds — instead of the municipal-level, yes/no hazard bands used today. It combines six public Italian geospatial sources (building geometry, official hazard maps, hydrography, elevation, and historical landslide/flood events) with two separate machine learning models (Gradient Boosting / Random Forest), each trained on real historical events and explained through SHAP.

Built for independent brokers, loss adjusters, and small-to-mid-sized non-life insurers who currently rely on slow, manual, low-granularity risk assessments — a gap made urgent by Italy's 2024 mandatory catastrophe insurance law (L. 213/2023) and the upcoming climate risk requirements of Solvency II.

## Why AI instead of a GIS lookup?

A hazard band can't tell two buildings in the same zone apart, doesn't update as fast as real risk patterns change, and can't weigh multiple correlated factors (distance from watercourse, elevation, slope, historical event frequency) at once. A model trained on where events actually happened learns those weights from data instead of a fixed threshold.

## Project status

Business plan and technical architecture developed as part of the *Business and Project Management* course, MSc in Artificial Intelligence and Data Engineering — University of Pisa (A.Y. 2025/2026). Conceptual/architectural design; no trained model or implementation yet.

## Sources

Built on public Italian geospatial data: ISPRA/IdroGEO (PAI hazard maps, IFFI landslide inventory), TINITALY DEM (INGV), OpenStreetMap (buildings, hydrography), EM-DAT (historical flood events).
