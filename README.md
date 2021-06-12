
<img src="https://spatial.ucr.edu/images/UCR_logo_long.png" alt="UCR"
	title="University of California" width="300" height="50"  /> 

[![Gitter](https://badges.gitter.im/p280s21project3/community.svg)](https://gitter.im/p280s21project3/community?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge)

# PBPL 280 Project: Education and Environmental Justice
## Exposure to Respiratory Hazards and Educational Performance in the Riverside Unified School District, California: A Geospatial Analysis. ##


## :pushpin: Contributors
[Laura Shah](https://github.com/lsala010/)

[Esteban Villegas](https://github.com/evill092)

[Wajiha Noor](https://github.com/WawNun)

[Preeti Juturu](https://github.com/preetijuturu)

[Salvador Jr. Olguin](https://github.com/Salolg5)

------
## 📝 Project Documentation

- [Final Presentation](https://docs.google.com/presentation/d/1rp7JEXDTZyxcVlwDGPZybQEtdEnhNggBlO7OzcP2YGs/edit?usp=sharing) 
Project presentation slides

- [Project Guidelines](https://sergerey.org/pbpl280s21/projects.html)
Project guidelines from the course instructor.

-  [HackMD for Proposal Writeup](https://hackmd.io/@xSZKUBllSUCUfYxmgoh_yA/SyurmYCUd)
Project proposal manuscript
  
- [HackMD for Literature Review](https://hackmd.io/@Laura786/S15WsEJ__/edit)
Extensive Literature Review 
  
 - [Project Report](https://github.com/preetijuturu/p280s21project3/blob/main/Project_Documents/PBPL280%20Group%203%20Manuscript.pdf)
 A Final version of the project report in PDF format.
  
 
------

## :notebook: Project Notebooks

The following set of links is intented for the purpose of direction. Each link give is linked to a complete version of notebooks for the project.
Check description below to find the ideal version. 

<img src="https://upload.wikimedia.org/wikipedia/commons/thumb/5/54/Euclidean_Voronoi_diagram.svg/1200px-Euclidean_Voronoi_diagram.svg.png" alt="Voronoi"
	title="methods" width="30" height="30"  />  Voronoi Analysis Codebook	

- [Voronoi Analysis - Los Angeles Unified School District](https://github.com/preetijuturu/p280s21project3/blob/main/LAUSD_Data.ipynb)
This notebook contains the Voronoi analysis for EJ Respiratory Index and Educational outcome for Los Angeles Unified School District. Data from SEDA, NCES, EJSCREEN and ACS has been truncated to find the educational outcomes for each school in LAUSD. EJ Respiratory Index is mapped on to voronoi polygons along with the schools location. 

- [Voronoi Analysis - Riverside Unified School District](https://github.com/preetijuturu/p280s21project3/blob/main/RUSD_Vor.ipynb)
This notebook contains the Voronoi analysis for EJ Respiratory Index and Educational outcome for Riverside Unified School District.Data from SEDA, NCES, EJSCREEN and ACS has been truncated to find the educational outcomes for each school in RUSD. EJ Respiratory Index is mapped on to voronoi polygons along with the schools location. Two separate indices are derived using different approaches. 


- [Voronoi Method- Extensive Approach To Estimate Racial Composition](https://github.com/preetijuturu/p280s21project3/blob/main/NEW_RUSD_Vor_extensive.ipynb)
This notebook contains the Voronoi analysis for Racial Composition and Educational outcome for Riverside Unified School District (using extensive approach). Contains additional information on the racial composition in RUSD. Racial composition is divided into three main groups percentage white, blacks and hispanic from ACS.
 
<img src="https://base.imgix.net/files/base/ebm/ehstoday/image/2020/03/ehstoday_3468_epalogo.5e7e64160e169.png?auto=format&fit=crop&h=432&w=768" alt="EPA"
	title="EPA" width="50" height="30"  />  EPA EJSCREEN Codebook
	
 - [EJ Screen](https://github.com/preetijuturu/p280s21project3/blob/main/EJ__V2.ipynb)
This notebook contains methods to retrieve, clean, overlay and visualize EJ Screen Data.

<img src="https://edopportunity.org/images/social/seda-social-image-08.png" alt="SEDA"
	title="SEDA" width="50" height="30"  /> SEDA Codebooks

- [SEDA Covariates Level Codes](https://github.com/preetijuturu/p280s21project3/blob/main/Codebook/New_SEDA.ipynb)
This notebook contains methods to retrieve, clean, overlay and visualize SEDA covariates level data. Cross-sectional data was generated for the year 2019. This file contains information on school level racial composition, school type and additional variables.

- [SEDA Education Outcomes](https://github.com/preetijuturu/p280s21project3/blob/main/Education_SEDA.ipynb)
This notebook contains methods to retrieve, clean, overlay and visualize SEDA educational outcomes data. Cross-sectional data was generated for the year 2019. This file contains information on school level average test scores and additional learning outcomes.


Additional Information

- [Combined File for Additional Analysis](https://github.com/preetijuturu/p280s21project3/blob/main/Combined_File2.ipynb)

This file have additional information on how to retrieve data for the project on the following counties (Los Angeles, Orange and Riverside County). 



------

##  :clipboard: Data Sources
----
A complete list of the main data sources and code to retrieve data for the study.
 
1. National Center for Education Statistics 
 
   - [NCES](https://open.quiltdata.com/b/spatial-ucr/tree/nces/schools/) 

```
schools = gpd.read_parquet('s3://spatial-ucr/nces/schools/schools_1718.parquet')

```
2. The Educational Opportunity Project at Stanford University 

    - [SEDA](https://edopportunity.org/) 
  
```
SEDA = pd.read_csv("https://stacks.stanford.edu/file/druid:db586ns4974/seda_cov_school_poolyr_4.0.csv")

```
3. United States Environmental Protection Agency(EPA) EJSCREEN

    - [EPA](https://open.quiltdata.com/b/spatial-ucr/tree/epa/ejscreen/)
   
```
import quilt3
b = quilt3.Bucket("s3://spatial-ucr")
b.fetch("epa/ejscreen/ejscreen_2020.parquet", "./ejscreen_2020.parquet")
ejscreen = pd.read_parquet('ejscreen_2020.parquet')
```

 4. Census Bureau's TIGERLINE FILES
     - [Elementary School Districts]( http://www2.census.gov/geo/tiger/TIGER2010DP1/ELSD_2010Census_DP1.zip)
     - [Census Bureau's TIGER database documentation]( https://www.census.gov/programs-surveys/saipe/technical-documentation/methodology/school-districts/overview-school-district.html)
     - [See the boundary files on this page]( https://www.census.gov/geographies/mapping-files/2010/geo/tiger-data.html)

```
tracts = gpd.read_parquet("s3://spatial-ucr/census/acs/acs_2018_tract.parquet")
```
----
## :notebook: Project Notebooks

<img src="https://upload.wikimedia.org/wikipedia/commons/thumb/5/54/Euclidean_Voronoi_diagram.svg/1200px-Euclidean_Voronoi_diagram.svg.png" alt="Voronoi"
	title="methods" width="30" height="30"  />  VORONOI ANALYSIS CODEBOOKS
- [Voronoi Analysis - Los Angeles Unified School District](https://github.com/preetijuturu/p280s21project3/blob/main/LAUSD_Data.ipynb)
- [Voronoi Analysis - Riverside Unified School District](https://github.com/preetijuturu/p280s21project3/blob/main/RUSD_Vor.ipynb)
- [Racial Composition and Voronoi Method Visualization](https://github.com/preetijuturu/p280s21project3/blob/main/Voroni%20(2).ipynb)
- [Voronoi Method- Extensive Approach To Estimate Racial Composition](https://github.com/preetijuturu/p280s21project3/blob/main/NEW_RUSD_Vor_extensive.ipynb)
 
<img src="https://base.imgix.net/files/base/ebm/ehstoday/image/2020/03/ehstoday_3468_epalogo.5e7e64160e169.png?auto=format&fit=crop&h=432&w=768" alt="EPA"
	title="EPA" width="50" height="30"  />  EPA EJSCREEN CODEBOOK
	
 - [EJ Screen](https://github.com/preetijuturu/p280s21project3/blob/main/EJ__V2.ipynb)

<img src="https://edopportunity.org/images/social/seda-social-image-08.png" alt="SEDA"
	title="SEDA" width="50" height="30"  /> SEDA CODEBOOKS

- [SEDA Covariates Level Codes](https://github.com/preetijuturu/p280s21project3/blob/main/Codebook/New_SEDA.ipynb)
- [SEDA Education Outcomes](https://github.com/preetijuturu/p280s21project3/blob/main/Education_SEDA.ipynb)

ADDITIONAL COMBO FILES

- [Combined File for Additional Analysis](https://github.com/preetijuturu/p280s21project3/blob/main/Combined_File2.ipynb)
- [ Basic compiled version with RUSD](https://github.com/preetijuturu/p280s21project3/blob/main/EJ_Visualization.ipynb)

-------

## 🛠️ Additional Resources and Readings

Repository- Introduction to Geospatial Data Analysis with Python
- https://github.com/sjsrey/gdapy18

- [As 'diesel death zones' spread in California, pollution regulators place new rules on warehouse industry](https://phys.org/news/2021-05-diesel-death-zones-california-pollution.html)
 


  	

