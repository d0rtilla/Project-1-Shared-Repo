# Poverty's Effect on Mental Health
## Overiew
## Contents
- Main_Findings
    - mian_data_exploration.ipynb
    - main_data_analysis.ipynb
    - Clean_Data
        - suicide_vs_unemployemnet_clean.csv
        - suicide_vs_gdp_clean.csv
- Additional_Findings
    - suicide_vs_unemployment_state.ipynb
    - suicide_vs_gdp_state.ipynb
    - suicide_vs_ihdi_country.ipynb
    - Resources
        - state_unemployment_USBLS.csv
        - state_gdp_USDOC.csv
        - state_suicide_CDC.csv
        - country_ihdi_WHO.csv
## Project Proposal
Group Number: 5

Group Members: Jacob Douthett, Ben Johnson, Jae Neuharth, Andrew Sundquist

Proposed Topic: Poverty's effect on mental health.

Overview: We plan to study how diferent economic factors, specifically unemployment rate, affect suicide rate.
### Main Research Question
- Is there a correlation between a country's unemployment rate and suicide rate?
### Main Hypothesis
- Countries with higher unemployment rates have higher suicide rates.
### Main Datasets
- The [global health observatory api from the WHO](https://www.who.int/data/gho/info/gho-odata-api) provides global data on [suicide rates](https://ghoapi.azureedge.net/api/MH_12) for nearly 200 countries.
- The [world bank's api](https://datahelpdesk.worldbank.org/knowledgebase/articles/889392-about-the-indicators-api-documentation) provides global data on [unemployment rates](https://api.worldbank.org/v2/country/indicator/JI.UEM.1564.ZS?format=json) for over 150 countries.
### Additional Research Questions and Datsets
- Is there a correlation between a country's per capita GDP and suicide rate?
- Do the same correlations, such as GDP vs suicide rate, exist on US state level?
- Is inequality-adjusted human developement index (IHDI) correlated with suicide rate?
- The [world bank's api](https://datahelpdesk.worldbank.org/knowledgebase/articles/889392-about-the-indicators-api-documentation) also provides data on [per capita GDP](https://api.worldbank.org/v2/country/indicator/NY.GDP.PCAP.CD?format=json).
- [Suicide rates by state](Test/suicide_rate_state.csv) data can be downloaded from the [CDC's 'Wonder'](https://wonder.cdc.gov/) database. 
- [Per capita GDP by state](Test/states_2018_gdp.csv) data can be downloaded from [Data.gov](https://data.gov/).
- [IHDI by country](Test/IHDI_time_series.csv) data can be downloaded from [Human Development Project's Website](https://hdr.undp.org/data-center/documentation-and-downloads).
## Milestones
- Project proposal approval
    - Written proposal &check;
    - Instructor approval &check;
- Data acquisition and cleanup
    - Data sources Identified &check;
    - Data files/APIs created &check;
    - NA data removed, DFs merged ect. and can print DFs &check;
- Data manipulation
    - Filter, sort, groupby to get useful data out of DFs &check;
    - data.ipynb complete &check;
- Graph/Charts
    - Create all needed graphics &check;
- Regression Analysis
    - Perform regression tests &check;
- Written Analysis
    - analysis.ipynb complete
## Main Analysis and Findings
### Is there a correlation between a country's unemployment rate and suicide rate?
## Additional Analysis and  Findings
### Is there a correlation between a country's per capita GDP and suicide rate?
### Do the same correlations, such as GDP vs suicide rate, exist on US state level?
The main research question investigated the correlation between a country's unemployment and GDP vs it's Suicide Rate. Further investigation was performed at a state level using the `suicide_rate_state.csv`, and a dataset from the BEA in the `BEA_GDP_DATA_multiple_years.csv`. The combined data provided data points for all 50 states from the years 1999 to 2020.

The jupyter notebook, `State_Suicide_GDP.ipynb` utilized these datasets. There were a few interesting findings based on the results. 
+ The null hypothesis was rejected (low p value below 0.05) when looking at GDP and Suicide Rate such that there is a non-zero slope where higher GDP results in lower Suicide Rate. However there are a few items of note:
    - The R Value is quite low which may indicate that there is not a strong correlation or that the linear regression will NOT be a great predictor of data.
    - The combination of the low P value (p = 0.0057 < p = 0. 05), and the low R value (r = - 0.08) caused some confusion, but generally speaking this tells us that the data is quite noisy/variable. So even though there is an observable trend in the linear regression, a certain GDP amount may result in a wide range of different suicide rates.
    - All this information leads us to believe that GDP is NOT a great indicator or predictor of suicide rates, and that there are obviously many more factors at play when it comes to causes of suicide Rates.

One other interesting item of note is that when viewing GDP vs Suicide Rate at a singular state level(ie, looking at just Minnesota instead of all 50 states), there is a strong positive correlation between higher GDP and higher suicide rates which is the opposite of the negative correlation when looking at all states together. 
### Is inequality-adjusted human developement index (IHDI) correlated with suicide rate?