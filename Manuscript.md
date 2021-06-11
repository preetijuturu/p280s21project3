# Exposure to Respiratory Hazards and Educational Performance in the Riverside Unified School District, California: A Geospatial Analysis.

## Introduction
Situated in the Inland Empire region of California, Riverside County has some of the highest rates of particulate matter pollution throughout the state. With the American Lung Association grading Riverside County air quality an "F," coupled with its ranking of second worst air pollution in the state, it is clear that Riverside County residents are constantly exposed to high levels of aerosol pollutants. [1, 2] Air pollution, particularly exposure to particulate matter and respiratory hazards, have adverse impacts on human health. Air pollution exposure has been attributed to high rates of pediatric and adult asthma, cardiovascular disease and chronic obstructive pulmonary disease (COPD). [1] Regional agencies such as the South Coast Air Quality Management District have emerged in an effort to support communities impacted by poor air quality, especially since the topography of Southern California makes Riverside County more prone to negative health impacts due to smog collecting in the region, being blown in from Los Angeles. [3]

Though the effects of particulate matter exposure on health outcomes are well researched and documented, there is limited academic research on the impacts of respiratory hazard exposure and educational outcomes. Previous works have sought to find associations between air toxics exposure and decreased academic performance, primarily through a public health and environmental science lens.  In a study of school children in China, researchers found a significant association between air pollution, particularly levels of NO2, and poorer results on neurobehavioral tests designed to measure the children’s sensory, motor, and psychomotor functions. [4] Furthermore, existing literature has suggested that minority children, notably Hispanic and African-American children, are exposed to higher levels of air pollution in comparison to white children. [5, 6, 7] African-American children are exposed to air pollution at disproportionate rates, even higher than Hispanic children. [5]  Low income communities are also exposed to air pollution at higher rates. Academic studies have found that low-income California communities were exposed to PM 2.5 almost 10% higher than the state average of exposure. [7]

Pollutants that are suspected or known toxicants have been noted to have an effect on school performance surpassing socioeconomic (SES) variables, and that school performance and toxicant exposure is statistically significant. [8] Studies show that areas with higher levels of residential air toxics are associated with lower grade point averages, and that there is a correlation between respiratory risk and lower economic performance even after controlling for SES. [8, 9] These studies, however, fail to assess the correlation between air toxin exposure and educational outcomes from a geospatial perspective. Understanding and mapping the health geography of environmental hazards and educational outcomes, as well as assessing the spatial relationship between the two, are practical and may be used by policymakers to influence change in environmental policy if academic outcomes are low in regions with high levels of respiratory hazards. This work seeks to  assess the impacts of respiratory toxins on educational outcomes using spatial methods, which has yet to be done in an empirically rigorous manner. This is done by using Riverside Unified School District (RUSD) as a case study to understand whether air toxin exposure and academic performance are correlated. Through this study, we are able to assess the correlation using pure spatial sciences and contribute to the limited body of knowledge studying environmental toxin exposure and academic outcomes. 

## Materials and methods
This work draws from open data, software and open science; this is discussed in more detail throughout this section. This study relies on spatial data science and novel econometric methods to assess the relationship between respiratory toxin exposure and academic outcomes in RUSD.

### Data sources

Data sources used in this study are publicly available and free of cost. The 2020 Environmental Justice Screening and Mapping Tool (EJSCREEN) data provided by the U.S. Environmental Protection Agency was quintessential in assessing exposure to respiratory toxins. The EJSCREEN tool makes data on environmental and demographic data easily accessible to the public, and also integrates EPA's own unique environmental indexes. [10] To assess respiratory hazards, this study used the National Scale Air Toxics Respiratory Hazard Index, paired with the EPA's Environmental Justice (EJ) measure. This measure seeks to incorporate both environmental exposure with demographic factors such as race, income and disability; the study  used the EJ index for air toxics respiratory hazard index. Higher EJ index values for air toxics respiratory hazards imply that more low-income minorities are being impacted by respiratory air toxics. [10] To map this data onto census block groups within the boundaries of RUSD, we utilised two significant data sets. Data from the 2018 American Community Survey (ACS) was used to join EJSCREEN data to census block group data, so we would be able to view the EJ index for air toxics respiratory hazards per block group in the country. We also used the U.S. Department of Education's National Center for Education Statistics (NCES) data to map out the school district boundaries for RUSD. This data

and the school distruict boundaries provided by the Department of Education

The second dataset used was the NCES for the school district data from 2018 to 2019 academic school year. Specifically, this dataset entails the locations of the schools in a given school district. 

The third dataset, we implemented into our project is the ACS or American Community Survey from the year 2018. This dataset entails demographic variables []

The fourth dataset that we compiled is the SEDA data; this data entails standardized test scores that were collected from the 3rd grade to the 8th grade in math and reading language arts or RLA. The school years range from 2008 to 2009 and 2017 to 2018. 
Why did we select the outcome variable how was it measured/estimated in the code? 

### Combining environmental and educational datasets 

Our community focus was on Riverside County (located in California); thus, district data from the Riverside Unified School District (RUSD) were analyzed and after visualizing a clear pattern of distinct variations in environmental justice the Respiratory Hazards Index was selected. In addition, cross-sectional data for 2018 was obtained from multiple open sources. [what other sources?] Block group data from EPA Environmental Justice (EJ) Screen was combined with American Community Survey (ACS). Furthermore, using geospatial boundaries the Respiratory Hazard Index for RUSD was mapped. As this index included demographic and population variables, the racial composition, median household income, and total population were mapped separately for the purposes of providing visualizations. Once basic visualization was done at the block group level, we proceeded to include educational outcomes data. NCES dataframe was combined with SEDA data set to find point geometry for each school. Our resulting sample for RUSD has a total of 39 observations for the average test scores administered from the 3rd grade to the 8th grade in math and reading language arts. The educational outcomes were visualize and mapped on the block group boundaries.

### Spatial analysis 


By using EJSCREEN we are able to observe the accumulation of various block groups within the Riverside Unified School County through polygons or "buffer report" (EPA, 2021).

In addition, the voronio method was used in Map B; the benefits for using the voronoi method on a simple map visualization is due to the fact the methodology is consistent in mapping out the centroids (represented by a point) within polygons, based off of the location of other nearby polygons. 
 
 


## Results and discussion
This section shall contain the results as well as data visualizations, tables and analysis.
1. Visual legends overlaying  
2. Veroni results 
3. Correlation and Causation 

### Data and analytical limitations 

The EJSCREEN dataset from the EPA has its limitations. For example, the dataset has some "uncertain estimates"; specifcially, in small block groups (EPA, 2021). Although it has this limitation the dataset is recommended to use for sumarizing the data in big areas, so that it may cover multiple block groups. The second limitation is that the dataset does not provide all possible environmental impacts and demographics. The reasoning why that is the case is that there are many components within environmental factors that have not been assessed and included in national databases such as the quality of drinking water or indoor air quality. The third limiation is that the income percentages are estimates, they may be over or under estimates because the data does not count for all households from the U.S. Census. Furthermore, the variables calculated are for "each block group" except specific environmental indicators "for air quality" such as the air quality of particle matter or Ozones (EPA,2021). These air quality indicators were assess for each Census tract or block group. Lastly, when using EJSCREEN is it important to consider that the EJSCREEN dataset ultimatley represents a proxy for assessing the possible health impacts in the United States.  


### Future research and policy recommendations 
(Wajiha/Laura) 

Researchers and policy makers should consider doing in-depth studies, addressing whether or not existing environmental policies(such as the famous Cap and Trade Program) lead to better environmental outcomes. In addition, researchers should consider if the "better" environmental outcomes lead to better health outcomes, espeacially in students.

Ultimately, the nature of our research represents a proxy model to demonstrate whether school's test performance is associated with air toxic pollution exposure based off of geospatial location. Furthermore, our second policy recommendation is for researchers to use our documentaiton and methodolgies to not only replicate our study but expand it as well by analyzing other counties and, schools. A benefit for expansion our study is that researchers can estimate the geospatial visualization of air toxic pollution on other regions. Through our research we are laying the foundation for other researchers that are interested in environmental issues.  

*discuss whether the results were in line with existing research and anticipated results, how the study may be improved, policy recommendations (with research backing them) and highlighting the need of further research regarding environmental exposure and academic performance.*

After showcasing the results and discussing the policy recommendations, it is important to reiterate the importance of this study because the negative issues surrounding environmental air hazards and the impact on school performance is a highly neglected and under-researched exploration. Also, it is imperative that our study can be utilized as a way to further expand future research on this subject. Therefore, (will add/edit more later)

## Conclusion
(Salvador & Esteban) 
The relationship between environmental exposure on student academic performance is an emerging research study that remains incomplete. Our model can serve as a template for future research projects that highlights the important of implementing clean environmental policy standards and it's potential impacts on student achievement. There are a number of caveats to the association between environmental exposure and academic achievement. This too includes our research study where our topic is one function among many that can impact a student ability to do well in their school work. In other words, other functions such as parental involvement, quality of neighborhood, academic support, all serve other variables that can also show an association to student achievement. Showcasing our results and investing research resources can provide a breadth of knowledge that demonstrates a clearer picture of the extent how air toxins ultimately play its part in student academic achievement. 


## References
1. American Lung Association. State of the Air: Riverside [Internet]. American Lung Association. Available from: https://www.lung.org/research/sota/city-rankings/states/california/riverside
2. James I. Riverside County air quality ranked among worst [Internet]. The Desert Sun. Available from: https://www.desertsun.com/story/news/environment/2014/04/30/american-lung-association-riverside-county-worst-us/8500589/
3. South Coast Air Quality Management District. The Southland’s War on Smog: Fifty Years of Progress Toward Clean Air (through May 1997) [Internet]. South Coast Air Quality Management District.  Available from: https://www.aqmd.gov/home/research/publications/50-years-of-progress
4. Wang S, Zhang J, Zeng X, Zeng Y, Wang S, Chen S. Association of Traffic-Related Air Pollution with Children’s Neurobehavioral Functions in Quanzhou, China. Environmental Health Perspectives [Internet]. 2009 Oct 1;117(10). Available from: https://ehp.niehs.nih.gov/doi/full/10.1289/ehp.0800023
5. Chakraborty J, Zandbergen PA. Children at risk: measuring racial/ethnic disparities in potential exposure to air pollution at school and home. J Epidemiol Community Health. 2007 Dec;61(12):1074–9. 
6. Liu J, Lewis G. Environmental Toxicity and Poor Cognitive Outcomes in Children and Adults. J Environ Health. 2014;76(6):130–8. 
7. Reichmuth D. Inequitable Exposure to Air Pollution from Vehicles in California [Internet]. Massachusetts Institute of Technology; 2019 Jan. (Union of Concerned Scientists). Available from: https://www.ucsusa.org/resources/inequitable-exposure-air-pollution-vehicles-california-2019
8. Scharber H, Lucier C, London B, Rosofsky A, Shandra J. The consequences of exposure to developmental, neurological, and respiratory toxins for school performance: a closer look at environmental ascription in East Baton Rouge, Louisiana. Popul Environ. 2013 Dec 1;35(2):205–24. 
9. Pastor M, Morello-Frosch R, Sadd JL. Breathless: Schools, Air Toxics, and Environmental Justice in California. Policy Studies Journal. 2006;34(3):337–62. 
10. US EPA. EJSCREEN: Environmental Justice Screening and Mapping Tool [Internet]. US EPA. 2014. Available from: https://www.epa.gov/ejscreen
