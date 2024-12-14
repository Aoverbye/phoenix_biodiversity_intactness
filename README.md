# Analysis of Biodiversity Intactness Index (BII) for Maricopa County (Phoenix)

#### Amanda G. Overbye

### Purpose
This notebook performs an analysis of the Biodiversity Intactness Index (BII) for Maricopa County (Phoenix), comparing BII values for the years 2017 and 2020. The analysis utilizes the io-biodiversity dataset provided by Impact Observatory and Vizzuality, clipped to the boundary of Maricopa County. The goal is to explore changes in biodiversity intactness within the county over this time period.

### Data

- **io-biodiversity dataset**:
  The biodiversity data can be accessed through the io-biodiversity collection available on [Microsoft's Planetary Computer](https://planetarycomputer.microsoft.com/dataset/io-biodiversity). This dataset contains Biodiversity Intactness Index (BII) values at a 100-meter resolution for the years 2017–2020, provided by Impact Observatory and Vizzuality. To begin, you can use the pystac_client library to access the STAC catalog and download the relevant data for the desired area and time period.
  
- **Shapefile (tl_2016_04_tract.shp)**: The county shapefile was obtained from the [United States Census Bureau website](https://www.census.gov/geographies/mapping-files/time-series/geo/tiger-line-file.html) and contains Census tract boundaries for Arizona. The data was downloaded as a shapefile and placed into the project's data folder. The os library was used to generate an absolute filepath, and the shapefile was read into the project using the GeoPandas package via the gpd.read_file() method.

### Repository Structure
```bash
phoenix_biodiversity_intactness
├── README.md
├── biodiversity_phoenix.ipynb
└── data
    ├── subdivision
    │   ├── tl_2024_04_cousub.cpg
    │   ├── tl_2024_04_cousub.dbf
    │   ├── tl_2024_04_cousub.prj
    │   ├── tl_2024_04_cousub.shp
    │   ├── tl_2024_04_cousub.shp.ea.iso.xml
    │   ├── tl_2024_04_cousub.shp.iso.xml
    │   └── tl_2024_04_cousub.shx
    ├── tl_2016_04_tract.cpg
    ├── tl_2016_04_tract.dbf
    ├── tl_2016_04_tract.prj
    ├── tl_2016_04_tract.shp
    ├── tl_2016_04_tract.shp.ea.iso.xml
    ├── tl_2016_04_tract.shp.iso.xml
    ├── tl_2016_04_tract.shp.xml
    └── tl_2016_04_tract.shx
```

### Acknowledgements

The repository was created as part of an assignment for the University of California, Santa Barbara course EDS 220: Working with Environmental Datasets. Details of the assignment can be found at the [course website](https://meds-eds-220.github.io/MEDS-eds-220-course/assignments/final-project.html)

### References

Microsoft Planetary Computer, *STAC Catalog. Biodiversity Intactness*. [Dataset]. https://planetarycomputer.microsoft.com/dataset/io-biodiversity. Accessed 7 December, 2024.

United States Census Bureau. 2024. *Arizona County TIGER/Line Shapefiles*. [Dataset]. United States Census Bureau. https://www.census.gov/geographies/mapping-files/time-series/geo/tiger-line-file.html. Accessed 7 December, 2024.

Microsoft Planetary Computer, STAC Catalog. Biodiversity Intactness. [Dataset]. https://planetarycomputer.microsoft.com/dataset/io-biodiversity. Accessed 7 December, 2024.

United States Census Bureau. 2024. Arizona County TIGER/Line Shapefiles. [Dataset]. United States Census Bureau. https://www.census.gov/geographies/mapping-files/time-series/geo/tiger-line-file.html. Accessed 7 December, 2024.
