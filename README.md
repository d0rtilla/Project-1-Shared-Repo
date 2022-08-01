# Project-1-Shared-Repo
 
## Project Proposal
Group Number: 5

Group Members: Jacob Douthett, Ben Johnson, Jae Neuharth, Andrew Sundquist

Proposed Topic: Poverty's affect on mental health.

Overview: We plan to study how diferent economic factors such as unemployment rate, GDP and human development index (HDI) affect suicide rate.
### Main Research Question
- Is there a correlation between a country's unemployment rate and suicide rate?
### Main Hypothese
- Countries with higher unemployment rates have higher suicide rates.
### Main Datasets
- The [global health observatory api from the WHO](https://www.who.int/data/gho/info/gho-odata-api) provides global data on [suicide rates](https://ghoapi.azureedge.net/api/MH_12) for nearly 200 countries.
- The [world bank's api](https://datahelpdesk.worldbank.org/knowledgebase/articles/889392-about-the-indicators-api-documentation) provides global data on [per capita GDP](https://api.worldbank.org/v2/country/indicator/NY.GDP.PCAP.CD?format=json) and [unemployment rates](https://api.worldbank.org/v2/country/indicator/JI.UEM.1564.ZS?format=json) for over 150 countries.
### Additional Research Questions and Datsets
- Is there a correlation between a contry's per capita GDP and suicide rate?
- Do the same correlations exist, such as GDP vs suicide rate, on US state level?
- Is inequality-adjusted human developement index (IHDI) correlated with suicide rate?
- [Suicide rates by state](Test/suicide_rate_state.csv) data can be downloaded from the [CDC's 'Wonder'](https://wonder.cdc.gov/) database. 
- [Per capita GDP by state](Test/states_2018_gdp.csv) data can be downloaded from [Data.gov](https://data.gov/).
- [IHDI by country](Test/IHDI_time_series.csv) data can be downloaded from [Human Development Project's Website](https://hdr.undp.org/data-center/documentation-and-downloads).
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
