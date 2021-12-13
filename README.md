# DATA512: Final Project

## Goal
The purpose of the project is to analyze the impact of COVID-19 vaccine on rate of infection, hospitalizations, and death in in Fairfield County, Connecticut. This project will also investigate how the COVID-19 pandemic impacted the unemployment rate in my assigned county. This repository is the final submission for DATA 512: Human-Centered Design for Data Science at the University of Washington.

## Research Questions
The research questions I investigated in this analysis are: 
1. What is the correlation between vaccination and daily rate of COVID-19 infections?
2. What is the correlation between vaccination on hospitalization?
3. What is the correlation between vaccination on deaths?
4. What is the impact of COVID-19 pandemic on the unemployment rate in Fairfield County, Connecticut?

## Data Source
The datasets used in this analysis are: 
1. [COVID-19 Confirmed Cases by County](https://www.kaggle.com/antgoldbloom/covid19-data-from-john-hopkins-university)
2. [COVID-19 Deaths by County](https://www.kaggle.com/antgoldbloom/covid19-data-from-john-hopkins-university)
3. [COVID-19 Cases, Hospitalizations, and Deaths (By County)](https://data.ct.gov/Health-and-Human-Services/COVID-19-Cases-Hospitalizations-and-Deaths-By-Coun/bfnu-rgqt)
4. [COVID-19 Vaccinations in the United States,County](https://data.cdc.gov/Vaccinations/COVID-19-Vaccinations-in-the-United-States-County/8xkx-amqh)
5. [Unemployment Rate in Fairfield County, CT](https://fred.stlouisfed.org/series/CTFAIR1URN)
6. [Mask Use by County](https://github.com/nytimes/covid-19-data/tree/master/mask-use)
7. [Mask Mandates by County](https://data.cdc.gov/Policy-Surveillance/U-S-State-and-Territorial-Public-Mask-Mandates-Fro/62d6-pm5i)

## Data Description

#### COVID-19 Confirmed Cases
This data state included a column for counties in the United States, I just used my assigned county data

| Column | Description | Data Type|
| ---         |     ---      |          ---|
| Province_State   | Daily Dates    | int   |
| Connecticut.1   | Number of Confiremed Cases       | int     |

#### COVID-19 Deaths
This data state included a column for counties in the United States, I just used my assigned county data

| Column | Description | Data Type|
| ---         |     ---      |          ---|
| Province_State   | Daily Dates    | Number   |
| Connecticut.1   | Number of Deaths       | Number     |

#### COVID-19 Cases, Hospitalizations, and Deaths (By County)
| Column | Description | Data Type|
| ---         |     ---      |          ---|
| Date Updated   | Date dataset was last updated     | Date & Time    |
| County Code     | County Code       | Number     |
| County | County name | Text |
| Total Cases  | Sum of confirmed and probable COVID-19 cases     | Number    |
| Confirmed Cases    | Number of laboratory-confirmed COVID-19 cases      | Number     |
| Probable Cases | Number of probable COVID-19 cases| int |
| Total case rate|  Rate of total cases per 100,000| int |
| Hospitalization Cases   |  Number of patients currently hospitalized with COVID-19   | Number    |
| Total Deaths    | Sum of confirmed and probable COVID-19-associated deaths     | Number      |
| Confirmed Deaths | Number of confirmed COVID-19-associated deaths | Number |
| Probable Deaths  | Sum of probable COVID-19-associated deaths     | Number    |

#### COVID-19 Vaccinations in the United States,County
| Column | Description | Data Type|
| ---         |     ---      |          --- |
| Date	| Date data are reported on CDC COVID Data Tracker | data & time    | 
| FIPS	 | Federal Information Processing Standard State Code| Number |
| MMWR_week	 | MMWR Week | Number   |
| Recip_County	 | County of residence | Text|
| Recip_State	 | Recipient State | Text|
| Series_Complete_Pop_Pct	| Percent of people who are fully vaccinated (have second dose of a two-dose vaccine or one dose of a single-dose vaccine) based on the jurisdiction and county where recipient lives     | Number    |
| Series_Complete_Yes	| Total number of people who are fully vaccinated (have second dose of a two-dose vaccine or one dose of a single-dose vaccine) based on the jurisdiction and county where recipient lives | Number      |
| Series_Complete_12Plus	 | Total number of people 12+ who are fully vaccinated (have second dose of a two-dose vaccine or one dose of a single-dose vaccine) based on the jurisdiction where recipient lives | Number |
| Series_Complete_12PlusPop_Pct	| Percent of people 12+ who are fully vaccinated (have second dose of a two-dose vaccine or one dose of a single-dose vaccine) based on the jurisdiction where recipient lives   | Number    |
| Series_Complete_18Plus	 | Total number of people 18+ who are fully vaccinated (have second dose of a two-dose vaccine or one dose of a single-dose vaccine) based on the jurisdiction and county where recipient lives     | Number   |
| Series_Complete_18PlusPop_Pct	| Percent of people 18+ who are fully vaccinated (have second dose of a two-dose vaccine or one dose of a single-dose vaccine) based on the jurisdiction and county where recipient lives      | Number     |
| Series_Complete_65Plus	| Total number of people 65+ who are fully vaccinated (have second dose of a two-dose vaccine or one dose of a single-dose vaccine) based on the jurisdiction where recipient lives | Number |
| Series_Complete_65PlusPop_Pct	| Percent of people 65+ who are fully vaccinated (have second dose of a two-dose vaccine or one dose of a single-dose vaccine) based on the jurisdiction where recipient lives     | Number   |
| Completeness_pct	| Represents the proportion of fully vaccinated people whose Federal Information Processing Standards (FIPS) code is reported and matches a valid county FIPS code in the jurisdiction.       | Number    |
(The remaining rows in the vaccination dataset were dropped and not used in this analysis)

#### Unemployment Rate in Fairfield County, CT
| Column | Description | Data Type|
| ---         |     ---      |          --- |
| Date   | Date of unemployment rate reported on monthly bases     | Date & Time    |
| CTFAIR1URN     | Rate of unemployment in Fairfield County        | Number      |


#### Mask Use by County
| Column | Description | Data Type|
| ---         |     ---      |          --- |
| COUNTYFP  | The county FIPS code.     | Number   |
| NEVER | The estimated share of people in this county who would say never in response to the question “How often do you wear a mask in public when you expect to be within six feet of another person?”     | Number     |
| RARELY | The estimated share of people in this county who would say rarely | Number |
| SOMETIMES | The estimated share of people in this county who would say sometimes     | Number    |
| FREQUENTLY | The estimated share of people in this county who would say frequently      | Number   |
| ALWAYS | The estimated share of people in this county who would say always | Number |


#### Mask Mandates by County
| Column | Description | Data Type|
| ---         |     ---      |          --- |
| State_Tribe_Territory	| U.S. state, tribe, and territory names     | Text    |
| County_Name	| U.S. county names      | Text    |
| FIPS_State	| U.S. state FIPS codes | Number |
| FIPS_County	| U.S. county FIPS codes     | Number   |
| date	| Daily date in dataset     | Text   |
| order_code |  | Text |
| Face_Masks_Required_in_Public	| A requirement for individuals operating in a personal capacity to wear masks 1) anywhere outside their homes or 2) both in retail businesses and in restaurants/food establishments    | Text  |
| Source_of_Action	| Source where order was found     | Text      |
| URL	| URL of order language used to complete dataset | Text |
| Citation	| Citation for the order   | Text  |



## Analysis Process
### Tools and Libraries Used
1. Jupyter Notebook
2. Python
   - [Pandas](https://pandas.pydata.org/)
   - [NumPy](https://numpy.org/)
   - [Matplotlib](https://matplotlib.org/)
   - [Seaborn](https://seaborn.pydata.org/)
3. R
   - [ggpubr](https://cran.r-project.org/web/packages/ggpubr/index.html)

### Methodology
Please refer to the Jupyter notebook and the R files. The process is also documneted in the final project report

## Results
1. Is there a correlation between getting fully vaccinated and the number of daily confirmed COVID-19 cases? 
   Yes, there was a correlation between vaccination and COVID-19 cases. The increase in vaccination leads to the decrease of COVID-19 cases and lowers the rate      of infection.
2. Is there a correlation between vaccination and COVID-19 related hospitalizations?  
      I found that there was a linear correlation between the two; as the number of people who are fully vaccinated increases, the number of COVID-19 related           hospitalizations decreases.
3. Is there a correlation between vaccination and COVID-19 related deaths?  
	Yes, my analysis showed that increasing vaccination decreases COVID-19 deaths
4. Is there a correlation between COVID-19 cases and the unemployment rate in Fairfield County?  
   Yes, there is a correlation between unemployment and COVID-19 cases. The unemployment rate spiked significantly at the beginning of the pandemic and              stayed at higher rates than it was in 2018 and 2019


## License
This repository is licensed under the MIT License and all the data are public domain
