## Prioritizing potential aquaculture

This repository contains the details of the assignment 4 for the course EDS 223: Geospatial Analysis & Remote Sensing for the Master of Environmental Data Science (MEDS) program.

The assignment focuses on determining which Exclusive Economic Zones (EEZ) on the West Coast of the US are best suited to developing marine aquaculture for several species of oysters and a species of our choice.

### Background

Marine aquaculture has the potential to play an important role in the global food supply as a more sustainable protein option than land-based meat production. [Gentry et al.](https://www.nature.com/articles/s41559-017-0257-9) mapped the potential for marine aquaculture globally based on multiple constraints, including ship traffic, dissolved oxygen, and bottom depth. They found that global seafood demand could be met using less than 0.015% of the global ocean area2.

All analysis were done on R version 4.5.1 using the following libraries tidyverse, sf, here and tmap.

### Objective of the assignment

Determine the Exclusive Economic Zones (EEZ) on the West Coast of the US best suited to develop marine aquaculture for several species of oysters and a species of our choice. For this,
- create a function that has the following characteristics:
  - arguments:
      minimum and maximum sea surface temperature
      minimum and maximum depth
      species name
  - outputs:
      map of EEZ regions colored by amount of suitable area
        species name should be included in the map’s title

### Contents

This repository contains the following files 1. .gitignore 2. prioritizing-potential-aquaculture.Rproj 3. aquaculture_analysis.qmd 4. figs: visual representation that is derived from the raw data 5. README.md

**File Structure**

```
EDS223-HW3
└─── README.md
└─── qmd/Rmd/Proj files
└─── aquaculture_analysis.qmd # Name your file a title that is representative of your analysis!
|   .gitignore
    └───data
        └─── wc_regions_clean.shp
        └─── depth.tif
        └─── average_annual_sst_2008.tif
        └─── average_annual_sst_2009.tif
        └─── average_annual_sst_2010.tif
        └─── average_annual_sst_2011.tif
        └─── average_annual_sst_2012.tif
```

### Data

Due to its large size, the `data` folder is included in `.gitignore` and is not tracked by version control. For this assignment, the data were pre-downloaded and provided by the team. Details of the data sources and download links are as follows:

#### Data download link
To access the data, [click here](https://drive.google.com/file/d/1u-iwnPDbe6ZK7wSFVMI-PpCKaRQ3RVmg/view)

#### Data Source

**Species**
You can find information on species depth and temperature requirements on [SeaLifeBase](https://www.sealifebase.ca/search.php). We are thinking about the potential for marine aquaculture, so these species should have some reasonable potential for commercial consumption.

**Sea Surface Temperature**
We are using average annual sea surface temperature (SST) from the years 2008 to 2012 to characterize the average sea surface temperature within the region. The data we are working with was originally generated from [NOAA’s 5km Daily Global Satellite Sea Surface Temperature Anomaly v3.1.](https://coralreefwatch.noaa.gov/product/5km/index_5km_ssta.php)

**Bathymetry**
To characterize the depth of the ocean we are using the [General Bathymetric Chart of the Oceans (GEBCO).](https://www.gebco.net/data-products/gridded-bathymetry-data#area)

**Exclusive Economic Zones**
We designate maritime boundaries using Exclusive Economic Zones off of the west coast of US from [Marineregions.org.](https://www.marineregions.org/eez.php)

### Course Information

-   **Course Title:** [EDS 223 - Geospatial Analysis & Remote Sensing](https://eds-223-geospatial.github.io/)
-   **Term:** Fall 2025
-   **Program:** [UCSB Masters in Environmental Data Science](https://bren.ucsb.edu/masters-programs/master-environmental-data-science).

Teaching Team:

-   **Instructor:** [Annie Adams](https://github.com/annieradams)
-   **Teaching Assistant:** [Alessandra Vidal Meza](https://avidalmeza.com/)

Complete description for the homework can be found on the [Assignment-4](https://eds-223-geospatial.github.io/assignments/HW4.html)

#### **Author**: Aakriti Poudel