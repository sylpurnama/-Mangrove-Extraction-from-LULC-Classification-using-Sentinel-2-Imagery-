# 🌿 Mangrove Mapping and Quality Assessment Using Sentinel-2 Imagery

A Google Earth Engine (GEE) script designed for extracting and assessing mangrove ecosystems from Land Use/Land Cover (LULC) classifications based on Sentinel-2 satellite imagery. This tool enables automated identification of mangrove areas and evaluates their health, supporting coastal ecosystem monitoring and management.

## 🚀 Features

### Core Functionality

**Automated LULC Classification**
- Classifies satellite imagery into five land cover classes using a Random Forest algorithm:
  - 0: Water Bodies
  - 1: Non-Mangrove Vegetation
  - 2: Mangroves
  - 3: Built-up Areas
  - 4: Bare Land

**Mangrove Extraction**
- Isolates mangrove regions (Class 2) from the LULC results using spectral thresholds and morphological filtering techniques

**Quality Assessment**
- Applies NDVI-based analysis to classify mangrove health into different condition levels (e.g., healthy vs. degraded)

**Statistical Analysis**
- Calculates mangrove area, class-wise distribution, and classification accuracy metrics

**Multi-format Export**
- Outputs classification and analysis results as raster (GeoTIFF) and vector (Shapefile) formats for further GIS processing

## 📋 Requirements

- Google Earth Engine account
- Basic knowledge of JavaScript for GEE
- Study area with mangrove coverage

## 🔧 Installation & Setup

1. Open [Google Earth Engine Code Editor](https://code.earthengine.google.com/)
2. Copy and paste the script into the code editor
3. Define your study area using the geometry tools or coordinates
4. Adjust the date range for Sentinel-2 imagery collection
5. Run the script

## 📊 Methodology

### Data Collection
Training sample collection follows Campbell (2002) methodology, which recommends a minimum of 100 pixels per class, evenly distributed across the study area to ensure reliable classification accuracy.

### Classification Process
1. **Image Preprocessing**: Sentinel-2 imagery is filtered, masked for clouds, and composite images are created
2. **Training Data**: Ground truth samples are collected for each land cover class
3. **Random Forest Classification**: Machine learning algorithm classifies pixels based on spectral signatures
4. **Post-processing**: Morphological filtering removes noise and improves classification accuracy

### Quality Assessment
- **NDVI Analysis**: Normalized Difference Vegetation Index is calculated to assess vegetation health
- **Mangrove Condition**: Health classification based on NDVI thresholds specific to mangrove ecosystems
- **Accuracy Assessment**: Confusion matrix and accuracy metrics validation

## 📈 Example Outputs

### 🌈 False Color Composite (Sentinel-2)
![False Color Composite](https://github.com/sylpurnama/-Mangrove-Extraction-from-LULC-Classification-using-Sentinel-2-Imagery-/blob/main/1.png)

### 🗺️ LULC Classification Result
![LULC Classification](https://github.com/sylpurnama/-Mangrove-Extraction-from-LULC-Classification-using-Sentinel-2-Imagery-/blob/main/2.png)

### 🌳 Mangrove Extraction Result
![Mangrove Extraction](https://github.com/sylpurnama/-Mangrove-Extraction-from-LULC-Classification-using-Sentinel-2-Imagery-/blob/main/3.png)

## 📁 Output Files

- **Classification Raster**: GeoTIFF format containing LULC classification results
- **Mangrove Shapefile**: Vector format of extracted mangrove boundaries
- **Quality Assessment**: Mangrove health condition maps
- **Statistical Report**: Area calculations and accuracy metrics

## 🎯 Applications

- Coastal zone management
- Mangrove conservation planning
- Climate change impact assessment
- Biodiversity monitoring
- Ecosystem service valuation

## 📚 References

Campbell, J. B. (2002). *Introduction to Remote Sensing*. Guilford Press.

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request or open an Issue for:
- Bug fixes
- Feature enhancements
- Documentation improvements
- Additional validation datasets

## 📄 License

This project is licensed under the MIT License - see the LICENSE file for details.

## 📧 Contact

For questions or collaboration opportunities, please open an issue or contact the repository maintainer.

---

*This tool supports the United Nations Sustainable Development Goals, particularly SDG 14 (Life Below Water) and SDG 15 (Life on Land) through improved mangrove ecosystem monitoring.*
