# lemay-evs-data
Code Scripts for "Observational Evidence of the of Electric Vehicles on Impact Local Air Quality in the United States"

CONTACT
	Name: Amélie Lemay
	Institution: Massachusetts Institute of Technology
	Email: alemay@mit.edu

DATASET INFORMATION

Datasets for each of the following variables were retrieved from the sources listed under 'SOURCES'.

1. Air Pollution (1)
2. Emissions (2)
3. County Characteristics (3)
4. EV Registrations (4–11)

EV registration datasets for the following states were obtained via public records requests 
and supplied via email to the author: AR, AZ, MD, NV, UT, WA

All EV registration data by county FIPS code is provided in the csv file EV_data.csv. 
Individual state-level data files are compiled to produce EV_data.csv in the R script Datasets.R. 
Individual state-level files are provided in the folder 'datasets.'

SOURCES

1. 	U.S. Environmental Protection Agency, Air Quality System Data Mart [internet database]. 
	https://www.epa.gov/outdoor-air-quality-data.
2. 	U.S. Environmental Protection Agency. 2020 National Emissions Inventory (NEI) Data.
	https://www.epa.gov/air-emissions-inventories/2020-national-emissions-inventory-nei-data (2020).
3.	American Community Survey. DP04: Selected Housing Characteristics [dataset]. U.S. Census Bureau
	https://data.census.gov/all?q=dp04.
4.	California Open Data Portal. Vehicle Fuel Type Count by Zip Code [dataset]. 
	https://data.ca.gov/dataset/vehicle-fuel-type-count-by-zip-code (2024).
5.	Atlas Public Policy. State EV Registration Database [dataset]. 
	https://www.atlasevhub.com/materials/state-ev-registration-data/#data.
6.	The Office of the Illinois Secretary of State. Electric Vehicle Counts by County [dataset]. 
	https://www.ilsos.gov/departments/vehicles/statistics/electric/home.html (2025).
7.	Kentucky Transportation Cabinet DataMart. Kentucky Registered Vehicle Counts [dataset]. 
	https://datamart.kytc.ky.gov/.
8.	Maine Department of Environmental Protection. Vehicle Emissions and Greenhouse Gas Data [dataset]. 
	https://www.maine.gov/dep/air/mobile/vehicle-data.html.
9.	Minnesota Public Utilities Commission. Electric Vehicles in Minnesota [dataset]. 
	https://mn.gov/puc/activities/economic-analysis/electric-vehicles/.
10.	North Carolina Department of Transportation. ZEV Registration Data [dataset]. 
	https://www.ncdot.gov/initiatives-policies/environmental/climate-change/Pages/zev-registration-data.aspx.
11.	South Dakota Department of Revenue. Statistics [datasets]. https://sddor.seamlessdocs.com/sc/statistics/.


FILES

1. datasets.zip -- Required data
	a. Datasets from above sources
	b. near_road_active_12_24.csv (list of near-road NO2 monitoring sites)
	c. zipToCounty24.csv (ZIP code crosswalk file)
3. Scripts.zip -- R code scripts
 	a. Datasets.R -- Loads and formats datasets
 	b. T_S3_S4.R -- Performs regression analysis of the annual summary data (tables S3-S4)
	c. T_S5.R -- Performs regression analysis of the daily summary data for seasonal comparisons (table S5)
	d. T_S6.R -- Performs regression analysis by NOx:VOC ratio (table S6)
	e. T_S7.R -- Performs regression analysis of near-road and non-near-road sites (table S7)
	f. T_S8.R -- Performs regression analysis using clustered standard errors (table S8)

The R scripts must be run sequentially.

SOFTWARE

Analysis was performed in R version 4.4.2 using RStudio 2024.12.0+467.

AI USE
Chat GPT was queried for several lines of R code for data wrangling and plotting.
