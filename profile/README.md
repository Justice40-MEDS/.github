# Identifying Disadvantaged Communities Using Cumulative Environmental Burdens


This GitHub organization hosts the code and documentation used in a Capstone Project for the degree of Master of Environmental Data Science for the [Bren School of Environmental Science & Management, University of California, Santa Barbara](https://bren.ucsb.edu/). The code and documentation for the [CEJST+](https://apps.bren.ucsb.edu/justice40/en/) is contained in this repository.

A link to the [full summary](https://bren.ucsb.edu/projects/identifying-justice40-communities-based-cumulative-environmental-burdens) on the UCSB Bren website.

## Summary: 
In January 2021, the federal government launched the Justice40 Initiative, which aims to direct 40% of overall benefits from investments in climate, clean energy, affordable housing, workforce development, remediation, pollution reduction and clean water infrastructure to disadvantaged communities (DACs). As part of this initiative, the federal government created the Climate and Economic Justice Screening Tool (CEJST) to identify which communities (census tracts) are considered disadvantaged and in need of federal funding based on the presence of low-income status and at least one of eight burden categories. While CEJST includes a wide range of useful indicators to evaluate burdens and designate DACs, it relies on a binary classification scheme that identifies U.S. census tracts as either DACs or non-DACs. Specifically, CEJST does not include any measure that represents cumulative burdens or overall harm to communities that occurs due to a combination of climate, environmental, socioeconomic, and health-related burdens (Shrestha 2023). A DAC meeting multiple criteria or indicator thresholds is assigned the same designation as a DAC meeting a single criterion and does not receive any special prioritization for Justice40 funding. This inability to distinguish between areas with severe, moderate, or lower burdens hinders the model's effectiveness, as identified in the recent National Academies of Sciences, Engineering, and Medicine consensus report (NASEM 2024). This project seeks to improve CEJST’s model by assessing the cumulative impact of climate and environmental burdens across communities in the U.S. The project team will utilize spatial analytic tools to highlight geographic clusters of communities that are overburdened using a cumulative assessment. They will implement techniques such as Local Indicators of Spatial Association that can be used to identify census tract clusters with significantly higher or lower levels of burden (Ansen 1995, Bivand & Wong 2018; Chakraborty 2024). By analyzing and incorporating cumulative burdens using cutting-edge geospatial techniques, the revised screening tool will promote more meaningful and equitable investment into disadvantaged communities facing the greatest risk from climate change.

## Objectives:
This project aims to improve the federal government's methodology for identifying U.S. communities disproportionately affected by the impacts of climate change and environmental burdens. These improvements will lead to a more precise allocation of Justice40 funds. In order to achieve this goal the project will focus on the following objectives:

- Incorporate a cumulative burden assessment into the CEJST to account for multiple climate and environmental stressors.
  
- Implement spatial analysis techniques to identify and map hotspots of cumulative environmental and climate burdens.
  
- Document the racial, ethnic, and socioeconomic characteristics of disadvantaged communities in the U.S. experiencing disproportionately high exposure to climate and environmental burdens.

## Repositories:
- [data-analysis](https://github.com/Justice40-MEDS/data-analysis): Houses our data exploration and statistical hotspot analysis. Also contains visualization content for presentations. 
- [j40-cejst-2](https://github.com/Justice40-MEDS/j40-cejst-2): Repository that holds the Climate and Economic Justice Screening Tool, the components within the tool, and the pipeline to create the map tiles. 

## Data

| **Inputs**                           | **Source**                                                                                                                                                                                |
|--------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Percentage of individuals below 200% of Federal Poverty Line**            | US Census Bureau’s American Community Survey API ([Link](https://www.census.gov/data/developers/data-sets.html))                                                                           |
| **Climate change burden category** (expected agricultural loss rate, expected building loss rate, expected population loss rate, projected flood risk, projected wildfire risk) | Federal Emergency Management Agency’s (FEMA) National Risk Index ([Link](https://hazards.fema.gov/nri/data-resources))                                                                     |
| **Energy burden category** (energy cost, PM2.5) | Department of Energy (DOE)’s LEAD Tool from 2018 ([Link](https://www.energy.gov/scep/low-income-energy-affordability-data-lead-tool-and-community-energy-solutions))<br>EPA AirToxScreen ([Link](https://www.epa.gov/AirToxScreen)) |
| **Health burden category** (asthma, diabetes, heart disease, low life expectancy) | Centers for Disease Control and Prevention’s (CDC) PLACES data from 2016 - 2019 ([Link](https://www.cdc.gov/places/index.html))<br>CDC’s USALEEP ([Link](https://www.cdc.gov/nchs/nvss/usaleep/usaleep.html#data))                     |
| **Housing burden category** (historic under-investment, housing cost, lack of green space, lack of indoor plumbing, lead paint) | National Community Reinvestment Coalition (NCRC) dataset of formerly redlined areas ([Link](https://www.openicpsr.org/openicpsr/project/141121/version/V2/view))<br>HUD’s CHAS dataset ([Link](https://www.huduser.gov/portal/datasets/cp.html)) |
| **Legacy pollution burden category** (abandoned mine land, formerly used defense sites, proximity to hazardous waste facilities, proximity to superfund sites, proximity to Risk Management facilities) | DOI’s Abandoned Mine Land Inventory System (e-AMLIS) ([Link](https://www.osmre.gov/programs/e-amlis))<br>EPA’s EJScreen ([Link](https://www.epa.gov/ejscreen/technical-documentation-ejscreen))                                  |
| **Transportation burden category** (diesel particulate matter exposure, transportation barriers, traffic proximity and volume) | DOT’s Transportation Access Disadvantage ([Link](https://www.transportation.gov/priorities/equity/justice40/transportation-insecurity))                                                    |
| **Water and wastewater burden** (underground storage tanks and releases, wastewater discharge) | EPA’s UST Finder ([Link](https://www.epa.gov/ust/ust-finder))<br>EPA’s RSEI model ([Link](https://www.epa.gov/ejscreen/technical-documentation-ejscreen))                                   |
| **Workforce development burden** (linguistic isolation, low median income, poverty, unemployment, high school education) | US Census Bureau’s American Community Survey API ([Link](https://www.census.gov/data/developers/data-sets.html))                                                                            |
| **Tribal lands category** (Land Area Representation depicts the exterior of a Federal Indian land area) | Bureau of Indian Affairs’ Land Area Representation dataset ([Link](https://www.bia.gov/bia/ots/dris/bogs))                                                                                  |
| **Racial/Ethnic Data**               | US Census Bureau’s American Community Survey 5-Year Estimates ([Link](https://www.census.gov/data/developers/data-sets.html))                                                               |


## Authors
- [Josephine Cardelle](https://github.com/jocardelle)
  
- [Kat Le](https://github.com/katleyq)
  
- [Haylee Oyler](https://github.com/haylee360)
  
- [Kimberlee Wong](https://github.com/kimberleewong)

## Client/Advisor
- [Jayajit Chakraborty](https://bren.ucsb.edu/people/jayajit-chakraborty)

## Acknowledgements
This project could not have been completed without the support and guidance of these people:

Faculty Advisor & Client: Dr. Jayajit Chakraborty, Bren School of Environmental Science & Management

Capstone Advisor: Dr. Carmen Galaz García, Bren School of Environmental Science & Management

Special Thanks: Dr. Max Czapanskiy, Bren School of Environmental Science & Management. Juliet Cohen, Bren School of Environmental Science & Management. Abigail Vath Meyer, National Center Ecological Analysis and Synthesis

## References

Anselin, L. (1995), Local Indicators of Spatial Association—LISA. Geographical Analysis, 27: 93-115. https://doi.org/10.1111/j.1538-4632.1995.tb00338.x

Bivand, R.S., Wong, D.W.S. Comparing implementations of global and local indicators of spatial association. TEST 27, 716–748 (2018). https://doi.org/10.1007/s11749-018-0599-x

Centers for Disease Control and Prevention and Agency for Toxic Substances Disease Registry. 2022 Environmental Justice Index. Accessed October 16, 2024. https://www.atsdr.cdc.gov/placeandhealth/eji/index.html

Chakraborty J, 2024. Using Local Indicators of Spatial Association to Analyze the Environmental Justice Implications of Ambient Air Pollution in the United States. Environmental Justice. https://doi.org/10.1089/env.2023.0017 

Getis, A., & Ord, J. K. (1992). The Analysis of Spatial Association by Use of Distance Statistics. Geographical Analysis, 24(3), 189–206. https://doi.org/10.1111/j.1538-4632.1992.tb00261.x 

Livings, M. and Wu, A-M. (2020). Local Measures of Spatial Association. The Geographic Information Science & Technology Body of Knowledge (3rd Quarter 2020 Edition), John P. Wilson (Ed.). DOI: 10.22224/gistbok/2020.3.10

National Academies of Sciences, Engineering and Medicine (NASEM). (2024). Constructing Valid Geospatial Tools for Environmental Justice. Washington DC: The National Academy Press. https://doi.org/10.17226/27317 

Shrestha, R. (2023, March 18). CEQ’s Climate and Economic Justice Screening Tool Needs to Consider How Burdens Add Up. World Resources Institute. Retrieved October 16, 2024, from https://www.wri.org/technical-perspectives/ceq-climate-and-economic-justice-screening-tool-cumulative-burdens 


