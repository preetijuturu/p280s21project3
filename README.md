
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

- [Final Presentation](https://docs.google.com/presentation/d/1qLhLtxjq6XK-siDOcR44per9_hq1gRP0U5N7I24vXpM/edit?usp=sharing) 
Project Presentation

- [Project Guidelines](https://sergerey.org/pbpl280s21/projects.html)
 Guidelines from the Course Instructor.

-  [HackMD for Proposal Writeup](https://hackmd.io/@xSZKUBllSUCUfYxmgoh_yA/SyurmYCUd)
Project proposal for Our Final Project
  
- [HackMD for Literature Review](https://hackmd.io/@Laura786/S15WsEJ__/edit)
Literature Review
 
 - [Project Manuscript](https://github.com/preetijuturu/p280s21project3/blob/main/Manuscript.md)
   

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
 


  	

