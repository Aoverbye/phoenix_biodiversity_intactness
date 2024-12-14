# Analysis of Biodiversity Intactness Index (BII) for Maricopa County (Phoenix)

#### Amanda G. Overbye

### Purpose
This notebook performs an analysis of the Biodiversity Intactness Index (BII) for Maricopa County (Phoenix), comparing BII values for the years 2017 and 2020. The analysis utilizes the io-biodiversity dataset provided by Impact Observatory and Vizzuality, clipped to the boundary of Maricopa County. The goal is to explore changes in biodiversity intactness within the county over this time period.

### Data

- io-biodiversity dataset: The data consists of global biodiversity intactness estimates at 100-meter resolution for the years 2017 and 2020. Intactness estimates are based on a combination of abundance and compositional similarity .
- Shapefile (tl_2016_04_tract.shp): Census tract boundaries for Arizona from the U.S. Census Bureau, used to define the boundary of Maricopa County.

### Repository Structure

.
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

### References

Microsoft Planetary Computer, STAC Catalog. Biodiversity Intactness. [Dataset]. https://planetarycomputer.microsoft.com/dataset/io-biodiversity. Accessed 7 December, 2024.

United States Census Bureau. 2024. Arizona County TIGER/Line Shapefiles. [Dataset]. United States Census Bureau. https://www.census.gov/geographies/mapping-files/time-series/geo/tiger-line-file.html. Accessed 7 December, 2024.
