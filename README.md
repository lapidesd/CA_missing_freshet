# Supplementary code and data for: Missing snowmelt runoff following drought explained by root-zone storage deficits
Supporting data and code for Lapides et al., 20XX.

[![DOI](https://zenodo.org/badge/428774645.svg)](https://zenodo.org/badge/latestdoi/428774645)

Colab notebooks:

* [Relationship between April 1 SWE and spring runoff](https://colab.research.google.com/drive/1tv8kbIe9EY3vFdAQzbJTfE7RmDpM9uQG?usp=sharing)
* [Storage deficits and spring ET calculations](https://colab.research.google.com/drive/1hq-qqlIR_LuEyZ5s5RPddnqDLBo4M309?usp=sharing)
* [Regression and random forest models for spring streamflow](https://colab.research.google.com/drive/1jPtdcESsGPfB2H6MC-W7metpiFSqe799?usp=sharing)
* [Mass balance model of streamflow generation from snowmelt](https://colab.research.google.com/drive/197Hglpe3kkThdblSFz-9U9h63IvdQzE9?usp=sharing)
* [Demonstration of application of these methods to 6 watershed of economic importance in California](https://colab.research.google.com/drive/1_igz4g_mbTntAkPZv3SJGwnYIRUEEBFE?usp=sharing)


This directory includes:
* Data
    * MODIS_and_PRISM_data--directory containing one file for each study site with monthly data for: ET (mm) from MODIS (Running et al., 2017), P (mm) from PRISM (Daly et al., 2008; Daly et al., 2015), wy (water year), and sumP (mm) cumulative precipitation for water year to date
    * evaporative_stress_index--directory containing one file for each study site with monthly average ESI
    * modis_temperature--directory containing one file for each study site with monthly mean land surface temperature (degrees C) from MODIS
    * site_data_wy_totals--directory containing one file for each study site with water year totals for: P (mm), adjP (mm) precipitation that fell as rain, spring_rain (mm) precipitation that fell as rain in the spring, winter_P (mm) precipitation from October-March, total_swe (mm) sum of all positive changes in SWE, snowfall_t (mm) snowfall determined as precipitation that fell with average temperature was below freezing, springET (mm) ET from April-July, maxDeficit (mm) maximum root zone storage deficit during the water year, minDeficit (mm) minimum root zone storage deficit during the water year, octDeficit (mm) October 1 deficit, aprDeficit (mm) April 1 deficit.
    * WY_data_all_sites.csv--same columns as files in site_data_wy_totals but aggregated over all study sites
    * april_swe_study_sites_mm.csv--April 1 SWE (mm) from SNODAS (National Operational Hydrologic Remote Sensing Center, 2004) with a column for each study site
    * california_site_list.zip--shapefile with list of study sites and gage locations
    * california_site_watershed_boundaries.zip--shapefile with watershed boundaries for each study site
    * dwr_gages.zip--shapefile with list of 6 watersheds of economic importance in California
    * dwr_watershed_boundaries.zip--shapefile with watershed boundaries for 6 watersheds of economic importance in California
    * melt_rates.csv--Water year mean melt rate for each study site (columns), mm/day
    * snodas_basin_data1.csv--SNODAS data (National Operational Hydrologic Remote Sensing Center, 2004) processed for each study basin organized by date and USGS site ID with SWE (mm), snowmelt (mm), and sublimation (mm) for each timestep
    * spring_streamflow_mm.csv--total spring streamflow (April-July) at each study site (columns) as calculated from NWIS data (U.S. Geological Survey, 2021)
    * state_outline.zip--shapefile of US state boundaries
    * snodas_basin_dwr.csv--daily aggregated SNODAS SWE data (mm) for each of 6 watersheds of economic importance in California
    * swe_q_residuals_mm.csv--Residual (mm) from SWE-Q linear regression for each year in the study period
* Code
    * process_snodas_data_share.ipynb--Jupyter notebook with code for processing SNODAS data and producing a map of April 1 SWE/maximal deficit in California. This notebook requires changes to be run and is only meant for sharing methods.
    * basin_selection_and_summary.ipynb--Jupyter notebook with code used to select study sites by applying the criteria described in the supplement to the article. The data used for this notebook is not included in this repository. This notebook is only meant for sharing methods.

Large data files were used and produced for this publication. Most of these data are available from pre-existing sources. We share our maps of 10, 25, 50, 75, and 90th percentile of April 1 SWE across the contiguous USA on HydoSHARE: [April 1 SWE data](https://www.hydroshare.org/resource/4b940b8593a4416e954a47bbbc58c568/).


# References
Daly, Christopher, et al. "Physiographically sensitive mapping of climatological temperature and precipitation across the conterminous United States." International Journal of Climatology: a Journal of the Royal Meteorological Society 28.15 (2008): 2031-2064.

Daly, Christopher, Joseph I. Smith, and Keith V. Olson. "Mapping atmospheric moisture climatologies across the conterminous United States." PloS one 10.10 (2015): e0141140.

Lapides, Dana A, Hahm, W Jesse, Rempe, Daniella M, Dralle, David N. (20XX) "Missing snowmelt runoff following drought explained by root-zone storage deficits".

National Operational Hydrologic Remote Sensing Center. "Snow data assimilation system (SNODAS) data products at NSIDC." (2004).

Running, S. and Mu, Q. and Zhao, M. (2017). MOD16A2 MODIS/Terra Net Evapotranspiration 8-Day L4 Global 500m SIN Grid V006 [Data set]. NASA EOSDIS Land Processes DAAC. doi: [https://doi.org/10.5067/MODIS/MOD16A2.006](https://doi.org/10.5067/MODIS/MOD16A2.006).

U.S. Geological Survey (2021). National Water Information System data available on the World Wide Web (Water Data for the Nation).
