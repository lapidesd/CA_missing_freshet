# CA_missing_freshet
Supporting data and code for "TITLE OF PUBLICATION"

This directory includes:
* Data
    * MODIS_and_PRISM_data--directory containing one file for each study site with monthly data for: ET (mm) from MODIS, P (mm) from PRISM, wy (water year), and sumP (mm) cumulative precipitation for water year to date
    * evaporative_stress_index--directory containing one file for each study site with monthly average ESI
    * modis_temperature--directory containing one file for each study site with monthly mean land surface temperature (degrees C) from MODIS
    * site_data_wy_totals--directory containing one file for each study site with water year totals for: P (mm), adjP (mm) precipitation that fell as rain, spring_rain (mm) precipitation that fell as rain in the spring, winter_P (mm) precipitation from October-March, total_swe (mm) sum of all positive changes in SWE, snowfall_t (mm) snowfall determined as precipitation that fell with average temperature was below freezing, springET (mm) ET from April-July, maxDeficit (mm) maximum root zone storage deficit during the water year, minDeficit (mm) minimum root zone storage deficit during the water year, octDeficit (mm) October 1 deficit, aprDeficit (mm) April 1 deficit.
    * WY_data_all_sites.csv--same columns as files in site_data_wy_totals but aggregated over all study sites
    * april_swe_study_sites_mm.csv--April 1 SWE (mm) from SNODAS (National Operational Hydrologic Remote Sensing Center, 2004) with a column for each study site
    * california_site_list.zip--shapefile with list of study sites and gage locations
    * california_site_watershed_boundaries.zip--shapefile with watershed boundaries for each study site
    * 

Colab notebooks:

* [Relationship between April 1 SWE and spring runoff](https://colab.research.google.com/drive/1tv8kbIe9EY3vFdAQzbJTfE7RmDpM9uQG?usp=sharing)
* [Storage deficits and spring ET calculations](https://colab.research.google.com/drive/1hq-qqlIR_LuEyZ5s5RPddnqDLBo4M309?usp=sharing)
* [AICc analysis to find best model for spring Q](https://colab.research.google.com/drive/1jPtdcESsGPfB2H6MC-W7metpiFSqe799?usp=sharing)
* [Simple model of streamflow generation from snowmelt in the Sierra](https://colab.research.google.com/drive/197Hglpe3kkThdblSFz-9U9h63IvdQzE9?usp=sharing)

# References
National Operational Hydrologic Remote Sensing Center. "Snow data assimilation system (SNODAS) data products at NSIDC." (2004).
