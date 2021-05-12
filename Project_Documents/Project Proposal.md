
### Group Members: Ariana, Esteban Villegas, Laura Shah, Preeti, Salvador Jr. Olguin, Wajiha Noor
### Professor Rey
### PBPL 280
---
# Project Proposal  
## Exposure to respiratory hazards and elementary school performance: A comparison between two Inland Empire cities
### Spring 2021 
------

 
### 1. Introduction 
This project will utilize open-source spatial data science tools and data to assess and compare the relationship between school academic performance and exposure to respiratory hazards in Southern California.The aim our project is to conduct a comparative analysis at the school district level for Moreno Valley Unified School District and the Riverside Unified School District. Additionally, we will map out the Environmental Justice Index for Air toxins respiratory hazards in Riverside and Moreno Valley in order to find if there is an association between school performance and geographic proximity to schools that are situated in high hazard locations.

### 2. Data

Necessary data sets will be sourced from the U.S. Environmental Protection Agency (EPA), the U.S. Department of Education and Stanford University. Most of the data sets and data infrastructure are preloaded to the UCR Center for Geospatial Science's Quilt data portal. This study will use the EPA’s “environmental justice” index for air toxins respiratory hazards to ensure that exposure to respiratory toxins is being viewed through a more comprehensive lens, taking into account income distributions and racial/ethnic composition of regions. Table 1 contains the list of all data type and the relevant sources.

#### Table 1: List of Data and Sources
| Data Type  | Source Links |   
|---|---|
| EJ Index for Air toxics respiratory hazard index  | https://open.quiltdata.com/b/spatial-ucr/tree/epa/ejscreen/ |
| Percentile for EJ Index for Air toxics respiratory hazard index| https://open.quiltdata.com/b/spatial-ucr/tree/epa/ejscreen/   |   
| Map color bin for EJ Index for Air toxics respiratory hazard index  | https://open.quiltdata.com/b/spatial-ucr/tree/epa/ejscreen/   |   
|Map popup text for EJ Index for Air toxics respiratory hazard index|https://open.quiltdata.com/b/spatial-ucr/tree/epa/ejscreen/|
|Test score trends |https://edopportunity.org/ |
|School district identification number |https://open.quiltdata.com/b/spatial-ucr/tree/nces/schools/ | 
|Name of institution|https://open.quiltdata.com/b/spatial-ucr/tree/nces/schools/||
|State FIPS| https://open.quiltdata.com/b/spatial-ucr/tree/nces/schools/ | 
|County FIPS|https://open.quiltdata.com/b/spatial-ucr/tree/nces/schools/|
|County name|https://open.quiltdata.com/b/spatial-ucr/tree/nces/schools/| 


### 3. Project Goal and Logistics 

- [x] Creating a GitHub repository for the project.
- [x] Researching literature on environmental exposure and its impacts on educational outcomes (See Appendix for references).
- [ ] Comparing  different school districts within the Inland Empire to check for variation in environmental hazards, income (socioeconomic status) , and educational outcomes such as test score trends, average test scores, and learning rates.
- [ ] Visualization and mapping of educational outcomes for school districts in Riverside as well as Moreno Valley and their relationship to environmental exposure. 
- [ ] Drafting a manuscript that combines the analysis, literature review and subsequent outcomes. 
- [ ] Creating documentation on Jupyter Notebook to ensure reproducibility of our work.


### 4. Project Milestones

- Project progress will be tracked via GitHub; project repository can be accessed via [github](https://github.com/preetijuturu/PBPL280-Education-and-EJ). 

###  Project Timeline

----
1. **Project Proposal Submission**: Project Proposal on HackMD.
`May 5, 2021`

2. **Project Milestone 1**: Paper Outline/ Literature Review & Basic Visualization.
`May 19, 2021 `

3. **Project Milestone 2**: Complete Data Analysis and Visualization.
`May 26, 2021 `

4. **Final Submission**: Manuscript and Project Reproducibility Documentation. 
`June 4, 2021`
----

### Questions for the instructor: 

1. Accessing data from EPA? 
2. How to combine SEDA data into the notebook?


---
## Appendix 

### References 
1. Clark-Reyna, S. E., Grineski, S. E., & Collins, T. W. (2016). Residential exposure to air toxics is linked to lower grade point averages among school children in El Paso, Texas, USA. Population and environment, 37(3), 319-340.

2. Grineski, S. E., Clark-Reyna, S. E., & Collins, T. W. (2016). School-based exposure to hazardous air pollutants and grade point average: A multi-level  study. Environmental research, 147, 164-171.

3. Liu, J., & Lewis, G. (2014). Environmental toxicity and poor cognitive outcomes in children and adults. Journal of environmental health, 76(6), 130.

4. Mohai, P., Kweon, B. S., Lee, S., & Ard, K. (2011). Air pollution around schools is linked to poorer student health and academic performance. Health Affairs, 30(5), 852-862.

5. Pastor Jr, M., Morello‐Frosch, R., & Sadd, J. L. (2006). Breathless: schools, air toxics, and environmental justice in California. Policy Studies Journal, 34(3), 337-362.

6. Pastor Jr, M., Sadd, J. L., & Morello-Frosch, R. (2004). Reading, writing, and toxics: children's health, academic performance, and environmental justice in Los Angeles. Environment and Planning C: Government and Policy, 22(2), 271-290.

7. Rosofsky, A., Lucier, C. A., London, B., Scharber, H., Borges-Mendez, R., & Shandra, J. (2014). Environmental ascription in Worcester County, MA:  toxic pollution and education outcomes. Local environment, 19(3), 283-299.

8. Scharber, H., Lucier, C., London, B., Rosofsky, A., & Shandra, J. (2013). The consequences of exposure to developmental, neurological, and respiratory toxins for school performance: a closer look at environmental ascription in East Baton Rouge, Louisiana. Population and Environment, 35(2), 205-224.
