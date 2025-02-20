# Road-crash
# Nairobi Road Analysis Project

This project analyzes road crash data in Nairobi, including geospatial visualization, road name standardization, and exploratory data analysis (EDA). Below is a comprehensive guide to set up and run this project.

---

## Requirements

### 1. **Environment**
- Python 3.12
- jupyter notebook

### 2. **Dependencies**

Install the following Python libraries:

```bash
pip install pandas numpy geopandas matplotlib seaborn folium shapely openpyxl
```

### 3. **Data**
#### Required Files:
- `filtered_latitude_longitude_rows.xlsx`: The cleaned dataset containing road data.
- Nairobi shapefile:
  - Download from one of the following:
    - [Geofabrik](https://www.geofabrik.de/)
    - [Kenya Open Data Portal](https://opendata.go.ke/)
    - [Humanitarian Data Exchange (HDX)](https://data.humdata.org/)
    - [GADM](https://gadm.org/)
  - Ensure the shapefile includes:
    - `.shp` (geometry)
    - `.shx` (shape index)
    - `.dbf` (attribute data)
    - `.prj` (projection data)

---

## Setup Instructions

1. Clone the repository:
   ```bash
   git clonehttps://github.com/barrack81/Road-crash
   cd (the directory you want to use)
   ```

2. Set up a virtual environment (optional but recommended):
   ```bash
   python -m virtualenv .venv
   source venv/bin/activate   # On Windows: venv\Scripts\activate
   ```

3. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

4. Place the required data files in the appropriate directories:
   - `cleaned.xlsx`: In the root project directory.
   - Nairobi shapefile components (`.shp`, `.shx`, `.dbf`, `.prj`): In a subdirectory named `shapefiles/`.(shapefiles currently not available)

---

## Running the Project

1. **Preprocessing and Cleaning:**
   - Standardize road names and filter rows with longitude and latitude data.

2. **Exploratory Data Analysis (EDA):**
   - Generate visualizations, such as bar charts, scatter plots, and heatmaps.

3. **Geospatial Analysis:**
   - Map crash locations and calculate distances from the Nairobi city center.

To execute the project:

```bash
python main.py
```

---

## Features

- **Data Cleaning:**
  - Standardizes road names for consistent analysis.
  - Filters rows with valid longitude and latitude values.

- **EDA:**
  - Provides statistical insights and visualizations of the dataset.

- **Geospatial Visualizations:**
  - Displays crash locations on an interactive map.
  - Calculates distances from the Nairobi city center.

---

## Additional Notes

- Ensure all dependencies are installed before running the scripts.
- Use `geopandas` for advanced geospatial analysis and `folium` for interactive maps.
- If shapefiles are not directly available, extract Nairobi-specific data using GIS tools like **QGIS** or **ogr2ogr**.

---

## Contact
For questions or issues, please contact Barrack Roy at barrackroy81@gmail.com. Whatsapp +254719733976
