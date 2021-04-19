# socio-economic-profiles

This code creates the socio-economic profile data for the San Francisco Planning Department's Neighborhood Socio-Economic Profiles. Socio-economic profiles data is derived from the American Community Survey 5-year data and is created annually by the Planning Department. Tract level socio-economic data from is combined at the neighborhood and district level for the City of San Francisco. This code is based off methods created by Michael Webster and others. The code is packaged in a Jupyter Notebook. 

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
