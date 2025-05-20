
# Climate Vulnerability Modelling in Morocco

This GitHub repository contains code for modeling climate vulnerability in Morocco, incorporating farmers' perceptions through survey data. The project is organized into three Jupyter Notebooks, which must be run in sequence. Each notebook should be used in combination with its corresponding dataset, stored in your own Google Drive.

---

## 📁 00 - Extraction of GEE Data

To use this notebook, follow these steps:

1. Load the shapefile from the `Data` folder: `MOROCCO_BOUNDARIES.zip`.
2. Unzip the file in your Google Drive.
3. Ensure you have an active Google Drive and Earth Engine account.

This script extracts multispectral indices and climate variables from Google Earth Engine (GEE), with a focus on the **Coefficient of Variation (CV)** for NDVI, temperature, and precipitation—key indicators for this project.

---

## 📊 01 - Data Analysis

This notebook requires the file `MOROCCO.csv`, which includes the survey data and the remote sensing variables extracted in the previous step.

The notebook performs:

- Descriptive statistics
- Visualization of key variables relevant to climate vulnerability

---

## 🔍 02 - Climate Vulnerability Modeling

This notebook also uses `MOROCCO.csv`. It performs the following steps:

- Data curation (removal of NA or blank entries)
- Category balancing
- Training of Random Forest and XGBoost classification models
- SHAP analysis for variable importance
- Comparison of models to identify the most influential and common variables across approaches

---

## 🧑‍💻 Contact

If you have any questions or feedback regarding the use of these notebooks, feel free to contact me:

**Dr. Cesar Ivan Alvarez**  
*Geospatial Engineering*  
📧 cesarivanalvarezmendoza@gmail.com
