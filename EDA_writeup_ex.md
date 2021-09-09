# CHOOSING COVID-19 VACCINE CENTERS BASED ON NYC SUBWAY STATIONS
Yazeed Musallam

## Abstract
The goal of the ministry of health is to end the pandemic as soon as possible. This can be achieved by a massive vaccination effort across the city and country and having herd immunity by 70% to prevent the disease from spreading. The primary goal of this project is to analyze where should the vaccination center be placed at, placing near to the NYC MTA subways is a great idea because 40% percent of NYC population uses the subway. I worked with MTA official data analyzing where should the vaccination center be placed at.
## Design
The ministry of health unsure where to put the vaccine spots as NYC is an enormous city, and the question arises to where the most effective spots could be with the limited budget.
The purpose of this analysis is to give insights into where the vaccine spots should be placed near to the most effective subway station to cut the costs and people can get vaccinated on the way to work or home, which can contribute to a higher overall vaccination rate in a shorter time and achieve the herd immunity.
After doing exploratory data analysis on the data; NYC Data Science will give a recommendation of where the vaccine spots should be placed.

## Data
Sample size:
> In the MTA dataset, the sample could be where the most crowded areas/subways and using the second dataset to verify where is the most crowded areas with the least amount of vaccinated people.
>  four months (May to August) of both datasets will be used for the analysis, and the reason is NYC started massive vaccine distrubution in the previous four months.

Description for the datset as num of rows, number of features/columns, names of columns with description:

Description of MTA Dataset:

> Number of rows: Approx. 3M rows

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
| STATION NAME      | Represents the station name        | object  |
| ZIPCODE   | Represent the the station zip code        | int64 |
## Algorithms

*Data cleaning*:
> 1) Fixing the reverse counter problem
> 2) Dealing with outliers

*Data validation*:
> 1) Checking no nulls
> 2) Checking no duplicates
> 3) Fixing turnstiles issue such as (reverse counter, zero counter turnstile, overshooting counter turnstile)

*Methodology of exploring the data*:
>	1)	Each subway station was mapped to percentage of fully vaccinated in that region, the analysis was done on only the subway stations areas with less than 65% fully vaccinated, filtering only to the busiest stations.
>	2)	Different analysis was implemented to answer the following questions in crowded stations with vaccination percentage less than 65%: 

>	  2.1) Are subway commuters in weekdays different than weekends? 
>	  2.2) Is there specific time the subway gets busy?

## Tools
The main technologies and libraries that used are:
Technologies:
> - Python
> - SQL
> - SQLite
> - Jupyter Notebook

Libraries:
> - Pandas
> - Matlibplot
> - SQL
> - Seaborn
> - SQLAlchemy 
> - NumPy

Processing tools: 
> Google Colab

## Communication
Findings:

<img src="https://raw.githubusercontent.com/YazeedMusallam/MTA-Project/main/images/barplotentries.png" width=500>
<img src="https://raw.githubusercontent.com/YazeedMusallam/MTA-Project/main/images/barplotvacc.png" width=500>
</br>
Slides are avaliable at:
</br>
https://github.com/YazeedMusallam/MTA-Project/blob/main/COVID-19%20VACCINE%20CENTERS%20SLIDES.pdf
<img src="https://raw.githubusercontent.com/YazeedMusallam/MTA-Project/main/images/slides.png" width=500>
