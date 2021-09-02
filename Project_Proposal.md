## Back story of the project:
The goal of the ministry of health is to end the pandemic as soon as possible. This can be achieved by a massive vaccination effort across the city and country and having herd immunity by 70% to prevent the disease from spreading.

NYC is a large city and getting to vaccine spots may be hard or the spots are placed in mostly vaccinated areas which contribute to end the pandemic in slower manner. About 40% of New Yorkers use the subway daily and focusing to get the people vaccinated who are going to work or home is a brilliant idea. Yet, ministry of health is unsure of where the vaccine spots should placed near to specific station.

The Ministry of health asked SDAIA for recommendation using data science to where should spots be placed. SDAIA proposed a solution to the ministry of health about where they should the vaccine spots should be placed near to most effective subway station.


## Background:
#### Company info:
> Saudi Authority for Data and Artificial Intelligence (SDAIA)

#### Problem statement:
> the Ministry of health unsure where to put the vaccine spots as NYC is an enormous city, and the question arises to where the most effective spots could be with the limited budget.

> The NYC MTA subway is used in about 40% of new yorkers, putting a vaccine spot near everywhere is infeasible due to over-budget (NYC has about 500 subway stations).
#### Value of the company and recommendations.
> The purpose of this analysis is to give insights into where the vaccine spots should be placed near to the most effective subway station to cut the costs and people can get vaccinated on the way to work or home, which can contribute to a higher overall vaccination rate in a shorter time and achieve the herd immunity.

> After doing exploratory data analysis on the data; SDAIA will give a recommendation of where the vaccine spots should be placed.
## Data Description:
* Datasets with description:
This project based on the following datasets:

> MTA Turnstile data located at http://web.mta.info/developers/turnstile.html.
The NYC MTA Turnstile data has cumulated number of entries and exits for each station in different dates and time. 

> Public NYChealth COVID-19 vaccine data located at https://github.com/nychealth/covid-vaccine-data.
The NYChealth COVID-19 vaccine data provides inforamtion about the vaccine percentage of each NYC district.

> MTA stations mapped to zipcodes dataset https://raw.githubusercontent.com/mvossbrinck/Metis_Project_1/04ab49df77000076e74e0ef90246bdbe2ac92775/female_male_ratio_subway_mapping.csv by github user: mvossbrinck
> This CSV file maps each station with it's corrsponding zip code.

## Scope of the work
Sample size:
> In the MTA dataset, the sample could be where the most crowded areas/subways and using the second dataset to verify where is the most crowded areas with the least amount of vaccinated people.
>  four months (May to August) of both datasets will be used for the analysis.

Description for the datset as num of rows, number of features/columns, names of columns with description:

Description of MTA Dataset:

> Number of rows: Approx. 193631 row / day

> Number of features/columns: 11 features/columns

> Names of columns with description:

| Columns     | Description | Data Type   |
| ----------- | ----------- | ----------- |
| C/A      | Control Area       | object  |
| UNIT   | Remote Unit for a station        | object|
| SCP      | Subunit Channel Position represents an specific address for a device       | object  |
| STATION   | Represents the station name the device is located at | object|
| LINENAME      | Represents all train lines that can be boarded at this station       |object  |
| DIVISION   | Represents the Line originally the station belonged to BMT, IRT, or IND        | object   |
| DATE   | Represents the date (MM-DD-YY)        | object   |
| TIME      | Represents the time (hh:mm:ss)     | object  |
| DESC   | Represent the "REGULAR" scheduled audit event (Normally occurs every 4 hours)        | object   |
| ENTRIES      | The comulative entry register value for a device       | int64|
| EXITS   | The cumulative exit register value for a device        | int64   |

Description of COVID-19 vaccine dataset:
> Number of rows: Approx. 177 row / day
 
> Number of features/columns: 13 features/columns

> Names of columns with description and type:

| Columns     | Description | Data Type   |
| ----------- | ----------- | ----------- |
| DATE      | Represents the date (MM-DD-YY)        | object  |
| NEIGHBORHOOD_NAME   | Neighborhood Name        | object|
| BOROUGH      | Administrative division  (i.e. Manhattan)     | object  |
| MODZCTA   | Zip code | int64|
| LABEL      | Multi zip codes       |object  |
| AGE_GROUP   | Category        | object   |
| POP_DENOMINATOR   | Number of population in the area | float64   |
| COUNT_PARTIALLY_CUMULATIVE      |   Cumulative number of at least had first dose   | int64  |
| COUNT_FULLY_CUMULATIVE   | Cumulative number who had fully dose        | int64   |
| COUNT_1PLUS_CUMULATIVE      |   Addition of the previous two columns     | int64|
| PERC_PARTIALLY   | Percentage of partially vaccinated        | float64   |
| PERC_FULLY   | Percentage of fully vaccinated        | float64   |
| PERC_1PLUS   | Addition of the previous two percentages        | float64   |

Description of station zip codes dataset:

> Number of rows: Approx. 315 row / day

> Number of features/columns: 2 features/columns

> Names of columns with description and type:

| Columns     | Description | Data Type   |
| ----------- | ----------- | ----------- |
| STOP NAME      | Represents the station name        | object  |
| ZIPCODE   | Represent the the station zip code        | int64 |



## Tools:
The main technologies and libraries that will be used are:
Technologies:
> - Python
> - SQL
> - SQLite
> - Jupyter Notebook

Libraries:
> - Pandas
> - Matlibplot
> - SQL

Note:
> During the project analysis, some additional tools may be used.

