
<img src="https://spatial.ucr.edu/images/UCR_logo_long.png" alt="UCR"
	title="University of California" width="300" height="50"  /> 

[![Gitter](https://badges.gitter.im/p280s21project3/community.svg)](https://gitter.im/p280s21project3/community?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge)

# 🌎 Education and Environmental Justice
## Exposure to Respiratory Hazards and Educational Performance in the Riverside Unified School District, California: *A Geospatial Analysis*. ##


## :pushpin: Contributors
[Laura Shah](https://github.com/lsala010/),  [Esteban Villegas](https://github.com/evill092),  [Wajiha Noor](https://github.com/WawNun),  [Preeti Juturu](https://github.com/preetijuturu),  [Salvador Jr. Olguin](https://github.com/Salolg5)

------
## 📁 Project Documentation

Proposal, report and slides for the project.

- [Final Presentation](https://docs.google.com/presentation/d/1qLhLtxjq6XK-siDOcR44per9_hq1gRP0U5N7I24vXpM/edit#slide=id.gdd58c2318c_3_178)
Open access project presentation (google slides).

-  [HackMD for Project Proposal](https://hackmd.io/@xSZKUBllSUCUfYxmgoh_yA/SyurmYCUd)
Project proposal manuscript (markdown format).
  
 - [Project Report](https://github.com/preetijuturu/p280s21project3/blob/main/Project_Documents/PBPL280%20Group%203%20Manuscript.pdf)
 A final version of the project report (PDF format).
  
  
------

## 📓 Project Reproducibility Documents

Methods and data analysis techniques for the project. 

### 📔  Data Retrieval Notebooks


####  `EPA-Environmental Justice Screen`
	
 - [EJ Screen](https://github.com/preetijuturu/p280s21project3/blob/main/EJ__V2.ipynb)
This notebook contains methods to retrieve, convert, overlay and visualize from EPA EJ Screen.

####  `SEDA-Educational Outcomes`

- [SEDA Covariates Level Codes](https://github.com/preetijuturu/p280s21project3/blob/main/Codebook/New_SEDA.ipynb)
This notebook contains methods to retrieve, convert, clean, overlay, and visualize SEDA covariates level data. Cross-sectional data was generated for the year 2019. The dataset includes information on school level racial composition, school type and additional variables provided by SEDA's educational opportunity website.

- [SEDA Education Outcomes](https://github.com/preetijuturu/p280s21project3/blob/main/Education_SEDA.ipynb)
This notebook contains methods to retrieve, convert, clean, overlay, and visualize SEDA educational outcomes data. The data covers averages values of learning outcomes for grades 3 to 8 over 2008-09 through 2017-18 school years. Information on school level educational outcomes such as average test scores and additional learning outcomes can be found in this file.


----
### 💻  Data Analysis Notebooks

The following set of links are intented to provide useful inforamtion on the data documents. Each link has a version of notebook generated for the purpose of geospatial data analysis and visualiation in python. Check description below to find the suitable version. 
	
####  `Voronoi Method `

- [Voronoi Analysis - EJ SCREEN for Riverside Unified School District](https://github.com/preetijuturu/p280s21project3/blob/main/RUSD_Vor.ipynb)
This notebook contains the voronoi analysis for EJ respiratory index and educational outcome using data from Riverside Unified School District(RUSD). Method to retrieve, merge and geosaptially analyze data from various sources including SEDA, NCES, EPA EJSCREEN and American Community Survery (ACS) is provided in this file. Environmental justice indicator such as respiratory hazard's index from EPA EJScreen is analyzed at block group level. Additionally the index is mapped onto voronoi polygons based on school locations from SEDA/NCES. Further estimation procedures such as areal interpolation and scatter plot are also part of the file.

- [Voronoi Method- Extensive Approach for Racial Composition](https://github.com/preetijuturu/p280s21project3/blob/main/NEW_RUSD_Vor_extensive.ipynb)
This notebook contains the voronoi analysis for racial composition and educational outcome using data from Riverside Unified School District. The file contains detail analysis of the racial composition indicators at block group levels within RUSD. Analysis is done for three main racial groups including NonHispanic Whites, Black and Hispanic population. The association between racial composition and educational outcomes is determined for each racial group separately.
 
####  `Material for Additional Analysis`

- [County Level Data](https://github.com/preetijuturu/p280s21project3/blob/main/Combined_File2.ipynb)
This file have additional information on how to retrieve NCES, SEDA, EJ Screen and ACS data for Los Angeles, Orange and Riverside County.

- [Voronoi Analysis - EJ Screen for Los Angeles Unified School District](https://github.com/preetijuturu/p280s21project3/blob/main/LAUSD_Data.ipynb)
This notebook contains the voronoi analysis for EJ Respiratory Index and Educational outcome for Los Angeles Unified School District. Data from SEDA, NCES, EJSCREEN and ACS has been truncated to find the educational outcomes for each school in LAUSD. EJ Respiratory Index is mapped on to voronoi polygons along with the schools location. 


------

##  📎 Open Data Sources

A complete list of open source data used in this project is linked below:
 
### 1. National Center for Education Statistics 
 
  - [NCES](https://open.quiltdata.com/b/spatial-ucr/tree/nces/schools/) 

```
schools = gpd.read_parquet('s3://spatial-ucr/nces/schools/schools_1718.parquet')
```
### 2. The Educational Opportunity Project at Stanford University 

  - [SEDA](https://edopportunity.org/) 
  
```
SEDA = pd.read_csv("https://stacks.stanford.edu/file/druid:db586ns4974/seda_cov_school_poolyr_4.0.csv")
```
### 3. United States Environmental Protection Agency(EPA) EJSCREEN

 - [EPA](https://open.quiltdata.com/b/spatial-ucr/tree/epa/ejscreen/)
   
```
import quilt3
b = quilt3.Bucket("s3://spatial-ucr")
b.fetch("epa/ejscreen/ejscreen_2020.parquet", "./ejscreen_2020.parquet")
ejscreen = pd.read_parquet('ejscreen_2020.parquet')
```

### 4. Census Bureau's TIGERLINE FILES
   - [Elementary School Districts]( http://www2.census.gov/geo/tiger/TIGER2010DP1/ELSD_2010Census_DP1.zip)
   - [Census Bureau's TIGER database documentation]( https://www.census.gov/programs-surveys/saipe/technical-documentation/methodology/school-districts/overview-school-district.html)
   - [See the boundary files on this page]( https://www.census.gov/geographies/mapping-files/2010/geo/tiger-data.html)

```
tracts = gpd.read_parquet("s3://spatial-ucr/census/acs/acs_2018_tract.parquet")
```
----



  	

