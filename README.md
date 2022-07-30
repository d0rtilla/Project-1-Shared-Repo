# Project-1-Shared-Repo
 
## Project Proposal
Group Number: 5
 
Group Members: Jacob Douthett, Ben Johnson, Jae Neuharth, Andrew Sundquist
 
Proposed Topic: Mental Health's Impact on Poverty
 
Overview: We plan to study how diferent economic factors such as unemployment rate, GDP and human development index (HDI) affect suicide rate.
 
### Questions
- Is there a correlation between a contry's per capita GDP and suicide rate?
- Is there a orrelation between a country's unemployment rate and suicide rate?
- Is there a correlation between state's per capita GDP and suicide rate?
 
### Hypotheses
- County's per capita GDP is negatively correlated with suicide rate.
- Country's unemployment rate is positively correlated with suicide rate.
- State's per capita GDP is negatively correlated with suicide rate.
 
### Datasets
- The [global health observatory api from the WHO](https://www.who.int/data/gho/info/gho-odata-api) provides global data on [suicide rates](https://ghoapi.azureedge.net/api/MH_12) for nearly 200 countries.
- The [world bank's api](https://datahelpdesk.worldbank.org/knowledgebase/articles/889392-about-the-indicators-api-documentation) provides global data on [per capita GDP](https://api.worldbank.org/v2/country/indicator/NY.GDP.PCAP.CD?format=json) and [unemployment rates](https://api.worldbank.org/v2/country/indicator/JI.UEM.1564.ZS?format=json) for over 150 countries.
- [Suicide rates by state](Test/suicide_rate_state.csv) data was downloaded from the [CDC's 'Wonder'](https://wonder.cdc.gov/) database. 
- [Per capita GDP by state](Test/states_2018_gdp.csv) data was downloaded from [Data.gov](https://data.gov/).

  
### Milestones
- Project proposal approval
    - Written proposal
    - Instructor approval
- Data acquisition and cleanup
    - Data sources Identified
    - Data files/APIs created
    - NA data removed, DFs merged ect. and can print DFs
- Data manipulation
    - Filter, sort, groupby to get useful data out of DFs
    - data.ipynb complete
- Graph/Charts
    - Create all needed graphics
- Regression Analysis
    - Perform regression tests
- Written Analysis
    - analysis.ipynb complete
