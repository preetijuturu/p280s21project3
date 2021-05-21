link: 
[What is EJSCREEN](https://www.epa.gov/ejscreen/what-ejscreen)

### What is EJSCREEN? 
* Environmental justice mapping and screening tool 
* Provides EP nationally consistent dataset 
* Combines environmental and demographics 
* EJSCREEN developed by EP 
    * Purpose: 
        * highlight places that has potential for "further review, analysis or outreach to support environmental justice work" 

**Includes:**  

* |11 environmental indicators|
    * https://www.epa.gov/ejscreen/overview-environmental-indicators-ejscreen
    * potential interests to project: (I believe this is the one that I selected)
        1. National-Scale Air Toxics Assessment (NATA) air toxics cancer risk
            * Lifetime cancer risk from inhalation of air toxics 
            * Data is from 2014 
            * Source: [EPA NATA](https://www.epa.gov/national-air-toxics-assessment/2014-nata-assessment-results) 
            
        2. NATA respiratory hazard index  
            * source: Air toxics respiratory hazard index (ratio of exposure concentration to health-based reference concentration)
            * Year: 2014 
        3. Traffic proximity and volume
            * Count of vehicles (AADT, avg. annual daily traffic) at major roads within 500 meters, divided by distance in meters (not km)
            * Calculated from 2017 U.S. Department of Transportation (DOT) traffic data,
            * retrieved 2019	2017
         4. * NATA diesel PM
             * Air
             * Diesel particulate matter level in air, µg/m3
             * EPA NATA
             * Data year 2014
* [6 demographic indicators](https://www.epa.gov/ejscreen/overview-demographic-indicators-ejscreen)
    * six demographic indicators:
    1. Percent Low-Income:
        * The percent of a block group's population in households where the household income is less than or equal to twice the federal "poverty level."
    2. Percent People of Color:
        * The percent of individuals in a block group who list their racial status as a race other than white alone and/or list their ethnicity as Hispanic or Latino. That is, all people other than non-Hispanic white-alone individuals. The word "alone" in this case indicates that the person is of a single race, not multiracial.
3. Less than high school education:
    * Percent of people age 25 or older in a block group whose education is short of a high school diploma.
4. Linguistic isolation:
    * Percent of people in a block group living in linguistically isolated households. A household in which all members age 14 years and over speak a non-English language and also speak English less than "very well" (have difficulty with English) is linguistically isolated.
5. Individuals under age 5:
    * Percent of people in a block group under the age of 5.
6. Individuals over age 64:
    * Percent of people in a block group over the age of 64.

* EJSCREEN includes an index that is based on the above demographic indicators:
    * A Demographic Index is based on the average of two demographic indicators; **Percent Low-Income and Percent Minority.**
* [11 EJ indexes](https://www.epa.gov/ejscreen/environmental-justice-indexes-ejscreen)
    * EJ index = combination of environmental and demographic info.
    * Eleven EJ Indexes in EJSCREEN reflecting the 11 environmental indicators.
        1. National Scale Air Toxics Assessment Air Toxics Cancer Risk
        2. National Scale Air Toxics Assessment Respiratory Hazard Index
        3. National Scale Air Toxics Assessment Diesel PM (DPM)
        4. Particulate Matter (PM2.5)
        5. Ozone
        6. Lead Paint Indicator
        7. Traffic Proximity and Volume
        8. Proximity to Risk Management Plan Sites
        9. Proximity to Treatment Storage and Disposal Facilities
        10. Proximity to National Priorities List Sites
        11. Wastewater Discharge Indicator


## [Limitations for EJSCREEN](https://www.epa.gov/ejscreen/limitations-and-caveats-using-ejscreen) 
### * **Disclosure:** 
* EJSCREEN not to be used for "detailed risk analysis" 
    * 1. Data in Demographic and environmental has "substantial uncertainty"  
        * specifically in **small areas**
        * SIngle block group mostly small and has "uncertain estimates" 
            * Recommend to, "Summarize EJSCREEN data within a larger area that may cover several block groups, in what is called a "buffer" report". 
    * 2. Does not provide data on **on every environmental impact and demographic indicator**
        * One reason is because: 
            * There are many environmental concerns not yet included in comprehensive, nationwide databases. 
            * For example: Data on Environmental factors like drinking water quality and indoor qir quality 
* Estimates on Demographics: 
    * (ex: percent low-income, come from surveys, not a full census of all households). 
    * This means the Census Bureau may estimate that a block group is 30% low-income, for example, but it might actually be 20% or 40% in some cases.
    * All indicators calculated for **each block group**.
        *  "Only exception = certain environmental indicators for air quality (PM, ozone, and NATA indicators). Those air data were obtained for each Census tract, so each block group in a tract was assigned the same environmental indicator value, as described in the Technical Documentation."
* Environmental indicators, there's uncertainty screening-level proxies for actual health impacts. 
    * Also applicable to indecaotrs with direct estimate risk or hazards 
        Ex: Air toxics cancer risk indicator 
            * uncertain indicators: 
                * Emissions
                * Exposure 
                * Toxicity 
 ---                
 ### Variables
|GDB Fieldname |Description|
|---|---|
|OBJECTID| unique ID for block group in geodatabase| 
|Shape| coordinates defining the features| 
|ID| Census FIPS code for block group|
|ACSTOTPOP| Total population| 
|ACSIPOVBAS|Population for whom poverty status is determined|
|ACSEDUCBAS| Population 25 years and over|
|ACSTOTHH| Households (for linguistic isolation)|
|ACSTOTHU| Housing units (for % built pre-1960)|
|MINORPOP|count of people of color individuals| 
|MINORPCT| % people of color|
|LOWINCOME|count of low-income individuals|
|LOWINCPCT|% low-income| 
|LESSHS|	count of individuals age 25 or over with less than high school degree| 
|LESSHSPCT|	% less than high school|
|LINGISO|	count of households in linguistic isolation|
|LINGISOPCT|	% of households (interpreted as individuals) in linguistic isolation|
|UNDER5|	count of individuals under age 5|
|UNDER5PCT|	% under age 5|
|OVER64|	count of individuals over age 64|
|OVER64PCT|	% over age 64|
|PRE1960|	count of housing units built before 1960|
|PRE1960PCT|	% pre-1960 housing (lead paint indicator)|
|VULEOPCT|	"Demographic Index (based on 2 factors, % low-income and % people of color)"|
|VULEO|	intermediate variable used for the Demograpic Index|
|DISPEO|	intermediate variable used for the Demographic Index|
|DSLPM|	Diesel particulate matter level in air|
|**CANCER**|	Air toxics cancer risk**|
|RESP|	Air toxics respiratory hazard index|
|PTRAF|	Traffic proximity and volume|
|PWDIS|	Indicator for major direct dischargers to water|
|PNPL|	Proximity to National Priorities List (NPL) sites|
|PRMP	Proximity to Risk Management Plan (RMP) facilities|
|PTSDF|	Proximity to Treatment Storage and Disposal (TSDF) facilities|
|OZONE|	Ozone level in air|
|PM25|	PM2.5 level in air|
|D_LDPNT_2|	EJ Index for % pre-1960 housing (lead paint indicator)|
|D_DSLPM_2|	EJ Index for Diesel particulate matter level in air|
|**D_CANCR_2|	EJ Index for Air toxics cancer risk**|
|D_RESP_2|	EJ Index for Air toxics respiratory hazard index|
|D_PTRAF_2|	EJ Index for Traffic proximity and volume|
|D_PWDIS_2|	EJ Index for Indicator for major direct dischargers to water|
|D_PNPL_2|	EJ Index for Proximity to National Priorities List (NPL) sites|
|D_PRMP_2|	EJ Index for Proximity to Risk Management Plan (RMP) facilities|
|D_PTSDF_2|	EJ Index for Proximity to Treatment Storage and Disposal (TSDF) facilities|
|D_OZONE_2|	EJ Index for Ozone level in air|
|D_PM25_2|	EJ Index for PM2.5 level in air|
|STATE_NAME|	Name of State|
|ST_ABBREV|	Two-letter abbreviation for State|
|REGION|	US EPA Region number|
|P_MINORPCT|	Percentile for % people of color|
P_LWINCPCT	Percentile for % low-income
P_LESHSPCT	Percentile for % less than high school
P_LNGISPCT	Percentile for % of households (interpreted as individuals) in linguistic isolation
P_UNDR5PCT	Percentile for % under age 5
P_OVR64PCT	Percentile for % over age 64
P_LDPNT	Percentile for % pre-1960 housing (lead paint indicator)
P_VULEOPCT	"Percentile for Demographic Index (based on 2 factors, % low-income and % people of color)"
P_DSLPM	Percentile for Diesel particulate matter level in air
**P_CANCR	Percentile for Air toxics cancer risk**
P_RESP	Percentile for Air toxics respiratory hazard index
P_PTRAF	Percentile for Traffic proximity and volume
P_PWDIS	Percentile for Indicator for major direct dischargers to water
P_PNPL	Percentile for Proximity to National Priorities List (NPL) sites
P_PRMP	Percentile for Proximity to Risk Management Plan (RMP) facilities
P_PTSDF	Percentile for Proximity to Treatment Storage and Disposal (TSDF) facilities
P_OZONE	Percentile for Ozone level in air
P_PM25	Percentile for PM2.5 level in air
P_LDPNT_D2	Percentile for EJ Index for % pre-1960 housing (lead paint indicator)
P_DSLPM_D2	Percentile for EJ Index for Diesel particulate matter level in air
P_CANCR_D2	Percentile for EJ Index for Air toxics cancer risk
P_RESP_D2	Percentile for EJ Index for Air toxics respiratory hazard index
P_PTRAF_D2	Percentile for EJ Index for Traffic proximity and volume
P_PWDIS_D2	Percentile for EJ Index for Indicator for major direct dischargers to water
P_PNPL_D2	Percentile for EJ Index for Proximity to National Priorities List (NPL) sites
P_PRMP_D2	Percentile for EJ Index for Proximity to Risk Management Plan (RMP) facilities
P_PTSDF_D2	Percentile for EJ Index for Proximity to Treatment Storage and Disposal (TSDF) facilities
P_OZONE_D2	Percentile for EJ Index for Ozone level in air
P_PM25_D2	Percentile for EJ Index for PM2.5 level in air
**B_MINORPCT	Map color bin for % people of color**
**B_LWINCPCT	Map color bin for % low-income**
**B_LESHSPCT	Map color bin for % less than high school**
**B_LNGISPCT	Map color bin for % of households (interpreted as individuals) in linguistic isolation** 
**B_UNDR5PCT	Map color bin for % under age 5**
B_OVR64PCT	Map color bin for % over age 64
B_LDPNT	Map color bin for % pre-1960 housing (lead paint indicator)
**B_VULEOPCT	"Map color bin for Demographic Index (based on 2 factors, % low-income and % people of color)"**
B_DSLPM	Map color bin for Diesel particulate matter level in air
**B_CANCR	Map color bin for Air toxics cancer risk**
B_RESP	Map color bin for Air toxics respiratory hazard index
B_PTRAF	Map color bin for Traffic proximity and volume
B_PWDIS	Map color bin for Indicator for major direct dischargers to water
B_PNPL	Map color bin for Proximity to National Priorities List (NPL) sites
B_PRMP	Map color bin for Proximity to Risk Management Plan (RMP) facilities
B_PTSDF	Map color bin for Proximity to Treatment Storage and Disposal (TSDF) facilities
B_OZONE	Map color bin for Ozone level in air
B_PM25	Map color bin for PM2.5 level in air
B_LDPNT_D2	Map color bin for EJ Index for % pre-1960 housing (lead paint indicator)
B_DSLPM_D2	Map color bin for EJ Index for Diesel particulate matter level in air
B_CANCR_D2	Map color bin for EJ Index for Air toxics cancer risk
B_RESP_D2	Map color bin for EJ Index for Air toxics respiratory hazard index
B_PTRAF_D2	Map color bin for EJ Index for Traffic proximity and volume
B_PWDIS_D2	Map color bin for EJ Index for Indicator for major direct dischargers to water
B_PNPL_D2	Map color bin for EJ Index for Proximity to National Priorities List (NPL) sites
B_PRMP_D2	Map color bin for EJ Index for Proximity to Risk Management Plan (RMP) facilities
B_PTSDF_D2	Map color bin for EJ Index for Proximity to Treatment Storage and Disposal (TSDF) facilities
B_OZONE_D2	Map color bin for EJ Index for Ozone level in air
B_PM25_D2	Map color bin for EJ Index for PM2.5 level in air
**T_MINORPCT	Map popup text for % people of color
**T_LWINCPCT	Map popup text for % low-income
**T_LESHSPCT	Map popup text for % less than high school
**T_LNGISPCT	Map popup text for % of households (interpreted as individuals) in linguistic isolation
**T_UNDR5PCT	Map popup text for % under age 5
T_OVR64PCT	Map popup text for % over age 64
T_VULEOPCT	"Map popup text for Demographic Index (based on 2 factors, % low-income and % people of color)"
T_LDPNT	Map popup text for % pre-1960 housing (lead paint indicator)
T_LDPNT_D2	Map popup text for EJ Index for % pre-1960 housing (lead paint indicator)
T_DSLPM	Map popup text for Diesel particulate matter level in air
T_DSLPM_D2	Map popup text for EJ Index for Diesel particulate matter level in air
T_CANCR	Map popup text for Air toxics cancer risk
**T_CANCR_D2	Map popup text for EJ Index for Air toxics cancer risk**
T_RESP	Map popup text for Air toxics respiratory hazard index
T_RESP_D2	Map popup text for EJ Index for Air toxics respiratory hazard index
T_PTRAF	Map popup text for Traffic proximity and volume
T_PTRAF_D2	Map popup text for EJ Index for Traffic proximity and volume
T_PWDIS	Map popup text for Indicator for major direct dischargers to water
T_PWDIS_D2	Map popup text for EJ Index for Indicator for major direct dischargers to water
T_PNPL	Map popup text for Proximity to National Priorities List (NPL) sites
T_PNPL_D2	Map popup text for EJ Index for Proximity to National Priorities List (NPL) sites
T_PRMP	Map popup text for Proximity to Risk Management Plan (RMP) facilities
T_PRMP_D2	Map popup text for EJ Index for Proximity to Risk Management Plan (RMP) facilities
T_PTSDF	Map popup text for Proximity to Treatment Storage and Disposal (TSDF) facilities
T_PTSDF_D2	Map popup text for EJ Index for Proximity to Treatment Storage and Disposal (TSDF) facilities
T_OZONE	Map popup text for Ozone level in air
T_OZONE_D2	Map popup text for EJ Index for Ozone level in air
T_PM25	Map popup text for PM2.5 level in air
T_PM25_D2	Map popup text for EJ Index for PM2.5 level in air
AREALAND	Land area in square meters
AREAWATER	Water area in square meters
NPL_CNT	Number of NPL facilities in the block group
TSDF_CNT	Number of TSDF facilities in the block group
Shape_Length	Shape length
Shape_Area	Shape area

 
### [NPL stands for National Priorities List](https://www.epa.gov/superfund/superfund-national-priorities-list-npl#:~:text=The%20National%20Priorities%20List%20%28NPL%29%20is%20the%20list,guide%20the%20EPA%20in%20determining%20which%20sites%20warrant)
* "The National Priorities List (NPL) is the list of sites of national priority among the known releases or threatened releases of hazardous substances, pollutants, or contaminants throughout the United States and its territories". 
* "The NPL is intended primarily to guide the EPA in determining which sites warrant further investigation."
