# Geothermal Project Documentation

## Project Overview
This project focuses on geothermal data analysis and visualization for Texas, including well data, temperature gradients, and zone mapping.

## Project Structure

### Data Directory
Contains all raw and processed data files organized into three main subdirectories:

#### 1. map_data_calc/
Contains calculation and analysis files for mapping purposes:

##### zones_of_intereest/
- `zones.ipynb`: Main notebook for zone analysis and categorization
- `zone_categories.csv`: Defines different geothermal zones and their characteristics
- `well_clusters_detailed_analysis.csv`: Contains detailed analysis of well clusters
- `wells_with_bht.xlsx`: Well data including Bottom Hole Temperature measurements

##### interpolation/
- `wells_with_interpolated_gradient.xlsx`: Contains interpolated gradient data for wells
- `texas_wells.csv`: Comprehensive well data for Texas
- `texas_gradient.csv`: Gradient calculations for Texas
- `texas_data.ipynb`: Notebook for Texas-specific data processing

##### BHT/
- `wells_with_interpolated_gradient.xlsx`: Interpolated gradient data
- `wells_with_bht.xlsx`: Well data with Bottom Hole Temperature
- `BHT.ipynb`: Notebook for Bottom Hole Temperature analysis

#### 2. wells_data/
Contains well-specific data and analysis:
- `well_in_texas.ipynb`: Main notebook for well data analysis and processing
- `wells in texas.xlsx`: Comprehensive well data in Excel format
- `texas_wells.csv`: Well data in CSV format for easier processing

*(Data source: [WellDatabase](https://welldatabase.com/))* ❗

#### 3. gradient_data/
Contains temperature and gradient-related data:

##### IRENA_temperature/
- `IRENA_hdr_T3km_global.tiff`: Temperature data at 3km depth
- `IRENA_hdr_T2km_global.tiff`: Temperature data at 2km depth
- `IRENA_hdr_T1km_global.tiff`: Temperature data at 1km depth
- `geothermal_data.ipynb`: Notebook for processing IRENA temperature data

*(Data source: [IRENA Global Atlas](https://globalatlas.irena.org/workspace))* ❗

Main files:
- `texas_data.csv`: Texas-specific temperature and gradient data
- `gradient.ipynb`: Main notebook for gradient calculations
- `geothermal_gradient.xlsx`: Comprehensive gradient data
- Depth-specific geothermal data files (1km, 2km, 3km)

### Maps Directory
Contains visualization and mapping files organized into three subdirectories:

#### 1. geothermal map/
- `map_gradient_from_xlsx.png`: Visualization of geothermal gradients
- `map.ipynb`: Notebook for generating gradient maps
- `wells_with_bht.xlsx`: Well data used for gradient mapping

#### 2. zones map/
- `map_zones.png`: Visualization of different geothermal zones
- `map.ipynb`: Notebook for zone mapping and visualization
- `zone_categories.csv`: Zone definitions and characteristics
- `well_clusters_detailed_analysis.csv`: Analysis used for zone mapping

#### 3. well map/
- `map_wells_density_green_red.png`: Well density visualization with color coding
- `map.ipynb`: Notebook for well mapping and density calculations
- `wells_with_bht.xlsx`: Well data used for mapping

## Data Processing Pipeline
1. **Data Collection**
   - Raw well data from Texas
   - Temperature data from IRENA
   - Bottom Hole Temperature measurements

2. **Data Processing**
   - Well data analysis and cleaning
   - Temperature gradient calculations
   - Zone categorization and analysis
   - Interpolation of missing data

3. **Visualization**
   - Gradient maps
   - Zone maps
   - Well density maps

## File Formats and Usage
- **Data Files**
  - CSV: For data processing and analysis
  - XLSX: For comprehensive data storage and sharing
  - TIFF: For temperature raster data

- **Analysis Files**
  - Jupyter Notebooks (.ipynb): For data processing and analysis
  - Python scripts: For specific calculations

- **Visualization Files**
  - PNG: For map visualizations
  - Interactive maps: Generated from notebooks

## Map Visualizations

### Geothermal Gradient Map
![Geothermal Gradient Map](Maps/geothermal%20map/map_gradient_from_xlsx.png)
*Map showing geothermal gradients across Texas*

### Well Density Map
![Well Density Map](Maps/well%20map/map_wells_density_green_red.png)
*Map showing well density distribution with color coding (green to red)*

### Zones Map **final result ⭐*
![Zones Map](Maps/zones%20map/map_zones.png)
*Map showing different geothermal zones in Texas*

## Dependencies
- Python 3.x
- Required Python packages:
  - pandas
  - numpy
  - matplotlib
  - folium
  - geopandas
  - rasterio (for TIFF processing) 
