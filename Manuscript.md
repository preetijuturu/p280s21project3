# Exposure to Respiratory Hazards and Educational Performance in the Riverside Unified School District, California: A Geospatial Analysis.

## Intro
This section contains the literature review elements in addition to reasoning behind the research topic selection

Research suggests that minorities, like Hispanic and African-American children are exposed to higher levels of air pollution in comparison to white children (Chakraborty & Zandbergen, 2007; Jianghong & Lewis, 2014; Reichmuth, David, 2019). In the study by Cakraborty and Zandbergen in 2007, pulled from more than 150,000 public schools from Orange County, Florida. Also, this study revealed that African American children were exposed more to air pollution compared to Hispanic Children. A study done in California concluded that African Americans, "on average...were exposed" to particle matter pollution at a rate of 43% higher than Whites. The particle matter pollution exposure rates for Latinos was on average 39% higher than Whites (Reichmuth, David, 2019). Race is one factor that is important to observe when researching environment justice policy issues. Another factor is income, specifically, low income communities that are exposed to air pollution are higher rates. In David Reichmuth's study in 2019, measured the particle matter (pm) pollution amongst the "lowest-income households" and found that these communities lived where the particle matter of 2.5 pollution" or "10 percent higher than the (California) state average" (Reichmuth, David, 2019.)  


Furthermore, the industrial industry are one of many producers of air toxins that significantly have adverse effects on human health outcomes. *insert more information about air toxins + citations)* Riverside County, the largest county in California's Inland Empire, is known for its high levels of air pollution and air toxics exposure. The effects of such exposure to human health such as respiratory function have been thoroughly examined, with the region notably containing rates of pediatric asthma that exceed California health and safety standards. (*insert citations here*) There is existing literature linking air toxics exposure to decreased academic performance. In a study of school children in China, researchers found a significant association between air pollution, particularly levels of NO2, and poorer results on neurobehavioral tests designed to measure the children’s sensory, motor, and psychomotor functions (Wang et al., 2009). It is important to note, however, that exposure to pollutants and decreased academic performance are not necessarily the result of SES variables. A recent study assessing the association between environmental toxicants and _____

## Importance:

The problems surrounding environmental air hazards and the impact on school performance is a highly neglected and under-researched exploration. Past literature review show individual studies in specific geographic regions testing the association between environmental inequality and that of academic performance indicators. Our group study supplements prior studied evidence that there is an environmental ascription in the sense that it can exert negative influence on academic performance in children and ultimately contribute to social inequalities. (Lucier, Rosofsky, London, Scharber, Shandra, 2011). We reveal that some schools and the students enrolled have an inherit attribute with these polluted environments. Our group study shows the importance of leveraging data from public sources and understanding and documenting the emerging relationship between environmental hazards against children's academic outcomes. Our study also brings to question who bears the brunt of the costs of environmental hazards as it matters to student academic outcomes and brings into question that the exploration between environmental hazards and academic outcomes remains unexamined/incomplete. We believe that with our group study, researchers and policymakers can utilize our model as a way to help expand further research that focuses on the relationship between environmental hazards and educational attainment.

Esteban (will add to this June 1, 2021)

## Data
This section shall contain information around the data sets, the methods, and why particular methods were used

(EJSCREEN-Preeti & Laura) 
The data used in our methods includes the EJScreen from the U.S. Environmental Protection Agency; specifically from the year 2020. The EJScreen data has valuable information on environmental justice data, indexes, and demographics. The selected index from EJSCREEN which accounted for both environmental and demographic data was the National Scale Air Toxics Respiratory Hazard Index. The EJ indicator that was used was D_RESP_2 and the demographic indicator pulled from EJSCREEN was the percent low-income. (This indicator refers to the block group population as it has information on areas "where the household income is less than or equal to twice the federal poverty level" (EPA, 2021). In addition, the other demographic indicator that was used was the "Percent People of Color"; the racial status or ethnitiy for only, blacks, Latino/Hispanic, and whites to represent the racial demographic was selected.    

The EJSCREEN dataset from the EPA has its limitations. For example, the dataset has some "uncertain estimates"; specifcially, in small block groups (EPA, 2021). Although, it has this limitation the dataset is recommended to use for sumarizing the data in big areas, so that it may cover multiple block groups. The second limitation is that the dataset does not provide all possible environmental impacts and demographics. The reasoning why that is the case is that there are many components within environmental factors that have not been assessed and included in national databases such as the quality of drinking water or indoor air quality. The third limiation is that the income percentages are estimates, they may be over or under estimates because the data does not count for all households from the U.S. Census. Furthermore, the variables calculated are for "each block group" except specific environmental indicators "for air quality" such as the air quality of particle matter or Ozones (EPA,2021). These air quality indicators were assess for each Census tract or block group. Lastly, when using EJSCREEN is it important to consider that the EJSCREEN dataset ultimatley represents a proxy for assessing the possible health impacts in the United States.  

The second dataset was used was the NCES for the school district data from 2018 to 2019 academic school year. Specifically, this dataset entails the locations of the schools in a given school district. 

The third dataset, we implemented into our project is the ACS or American Community Survey from the year 2018. This dataset entails demographic variables []

The four dataset that we complied is the SEDA data; this data entails standardized test scores that were collected from the 3rd grade to the 8th grade in math and reading language arts or RLA. The school years range from 2008 to 2009 and 2017 to 2018. 
Why did we select the outcome variable how was it measured/estimated in the code? 

## Methods: [Laura & Wajiha] 

Our community focus was on Riverside County (located in California); thus, district data from the Riverside Unified School District (RUSD) were analyzed and after visualizing a clear pattern of distinct variations in environmental justice the Respiratory Hazards Index was selected. In addition, cross-sectional data for 2018 was obtained from multiple open sources. [what other sources?] Block group data from EPA Environmental Justice (EJ) Screen was combined with American Community Survey (ACS). Furthermore, using geospatial boundaries the Respiratory Hazard Index for RUSD was mapped. As this index included demographic and population variables, the racial composition, median household income, and total population were mapped separately for the purposes of providing visualizations. Once basic visualization was done at the block group level, we proceeded to include educational outcomes data. NCES dataframe was combined with SEDA data set to find point geometry for each schools. Our resulting sample for RUSD has a total of 39 observations for the average test scorces administered from the 3rd grade to the 8th grade in math and reading language arts. The educational outcomes where visualize and mapped on the block group boundaries.

### Spatial analysis 


By using EJSCREEN we are able to observe the accumulation of various block groups within the Riverside Unified School County through polygons or "buffer report" (EPA, 2021).

In addition, the voronio method was used in Map B; the benefits for using the voronoi method on a simple map visualization is due to the fact the methodology is consistent in mapping out the centroids (represented by a point) within polygons, based off of the location of other nearby polygons. 
 
The limitation to using the voronoi method is that the formula does not account for neighborhood movements as it assumes the neighborhoods remain constant. 

The second limitation is 

## Results (pending) 
This section shall contain the results as well as data visualizations, tables and analysis.
1. Visual legends overlaying  
2. Veroni results 
3. Correlation and Causation 

## Policy Recommendation (generalize)
(Wajiha/Laura) 

Researchers and policy makers should consider doing in-depth studies, addressing whether or not existing environmental policies(such as the famous Cap and Trade Program) lead to better environmental outcomes. In addition, researchers should consider if the "better" environmental outcomes lead to better health outcomes, espeacially in students.

Ultimately, the nature of our research represents a proxy model to demonstrate whether school's test performance is associated with air toxic pollution exposure based off of geospatial location. Furthermore, our second policy recommendation is for researchers to use our documentaiton and methodolgies to not only replicate our study but expand it as well by analyzing other counties and, schools. A benefit for expansion our study is that researchers can estimate the geospatial visualization of air toxic pollution on other regions. Through our research we are laying the foundation for other researchers that are interested in environmental issues.  


## Discussion and conclusions 
(Salvador & Esteban) 
Restate the importance/relevance of the study:  
*This section shall discuss whether the results were in line with existing research and anticipated results, how the study may be improved, policy recommendations (with research backing them) and highlighting the need of further research regarding environmental exposure and academic performance.*

After showcasing the results and discussing the policy recommendations, it is important to reiterate the importance of this study because the negative issues surrounding environmental air hazards and the impact on school performance is a highly neglected and under-researched exploration. Also, it is imperative that our study can be utilized as a way to further expand future research on this subject. Therefore, (will add/edit more later)

## Work Cited 
1. Chakraborty J, Zandbergen PA. Children at risk: measuring racial/ethnic disparities in potential exposure to air pollution at school and home. J Epidemiol Community Health. 2007 Dec;61(12):1074-9. doi: 10.1136/jech.2006.054130. PMID: 18000130; PMCID: PMC2465656. 
2. Liu, Jianghong, and Gary Lewis. “Environmental toxicity and poor cognitive outcomes in children and adults.” Journal of environmental health vol. 76,6 (2014): 130-8.
3.  “Overview of Environmental Indicators in EJSCREEN.” EPA, Environmental Protection Agency, 5 Apr. 2021, www.epa.gov/ejscreen/overview-environmental-indicators-ejscreen. 
4.  Reichmuth, David. 2019. Inequitable Exposure to Air Pollution from Vehicles in California. Cambridge, MA: Union of Concerned Scientists. https://www.ucsusa.org/resources/inequitable-exposure-air-pollution-vehicles-california-2019
