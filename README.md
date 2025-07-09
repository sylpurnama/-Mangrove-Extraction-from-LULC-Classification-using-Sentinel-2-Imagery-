🌿 Mangrove Mapping and Quality Assessment Using Sentinel-2 Imagery
A Google Earth Engine (GEE) script designed for extracting and assessing mangrove ecosystems from Land Use/Land Cover (LULC) classifications based on Sentinel-2 satellite imagery. This tool enables automated identification of mangrove areas and evaluates their health, supporting coastal ecosystem monitoring and management.

🚀 Features
Core Functionality
Automated LULC Classification
Classifies satellite imagery into five land cover classes using a Random Forest algorithm:

0: Water Bodies

1: Non-Mangrove Vegetation

2: Mangroves

3: Built-up Areas

4: Bare Land

Mangrove Extraction
Isolates mangrove regions (Class 2) from the LULC results using spectral thresholds and morphological filtering techniques.

Quality Assessment
Applies NDVI-based analysis to classify mangrove health into different condition levels (e.g., healthy vs. degraded).

Statistical Analysis
Calculates mangrove area, class-wise distribution, and classification accuracy metrics.

Multi-format Export
Outputs classification and analysis results as raster (GeoTIFF) and vector (Shapefile) formats for further GIS processing.

📌 Sampling Guidelines
Training sample collection follows Campbell (2002), which recommends a minimum of 100 pixels per class, evenly distributed across the study area to ensure reliable classification accuracy.
