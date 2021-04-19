# socio-economic-profiles

This code creates the socio-economic profile data for the San Francisco Planning Department's Neighborhood Socio-Economic Profiles. Socio-economic profiles data is derived from the American Community Survey 5-year data and is created annually by the Planning Department. Tract level socio-economic data is combined at the neighborhood and district level for the City of San Francisco. This code is based off methods created by Michael Webster and others. Launch the Jupyter Notebook to calculate socio-economic profiles data, visualize results, and download.  

## Installation

Set up a [Python virtual environment](https://docs.python.org/3/library/venv.html) and activate

```bash
pip install virtualenv
python3 -m venv /path/to/new/virtual/environment/env
source env/bin/activate
```

Use the package manager [pip](https://pip.pypa.io/en/stable/) to install Python packages via requirements.txt.

```bash
pip install requirements.txt
```

To visualzed results on a map the Geopandas Python library is used. Geopandas requires special attention to install on Windows. Install Fiona, GDAL, Geopandas, pyproj, and Shapely via windows Binaries by following the instructions [here](https://towardsdatascience.com/geopandas-installation-the-easy-way-for-windows-31a666b3610f). Alternatively install Geopandas via Conda. 

## Usage

Launch the Jupyter Notebook
```bash
jupyter notebook
```

## Files
- /build_socioeconomic_profiles.ipynb: Python Notebook for calculating socio-economic profiles
- /Data_Items_And_Sources_2019.xlsx: Excel file containing attribute calculations that the python notebook calculations are based on
- /attribute_lookup.csv: Lookup table with attribute categories, attributes names and attribute IDs for all attributes needed to calcualte the profile data
- /geo_lookup.csv: Lookup table with neighborhood, supervisor district, and city name for each tract in San Francisco.  
- /median_lookup.csv: Lookup table needed for calculating medians. Contains name, id, range_start, and range_end for median calcs. 
- /neighborhoods/neighborhoods.shp: Shapefile with San Francisco Neighborhoods used for mapping visualization
- /supervisor_districts/supervisor_districts.shp: Shapefile with San Francisco Supervisor Districts for mapping visualization
