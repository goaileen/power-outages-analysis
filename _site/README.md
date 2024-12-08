# Power Outages Analysis ⚡️
<!-- Analyzing what areas are most affected by power outages. -->
<!-- How do features like residential electric prices affect how quickly/the duration of a power outage? -->

Homework 11 for EECS 398: Practical Data Science at U-M

Aileen Gonzalez

# Introduction
The dataset this analysis is applied on has major power outage data in the continental US from January 2000 to July 2016. Major power outages are defined, by the Department of Energy, as impacting at least 50,000 customers or causing an unplanned firm load loss of at least 300 MW.

This data presents information on geographical location, date time, regional climates, land-use, electricity consumption patterns, and economic characteristics of the states affected by the outages.

Considering the data available, this analysis seeks to address the question:

### **"Does the cost of electricity and the setting of residents (urban/rural population) influence the duration and severity (number of customers affected) of major power outages?"**

This question seeks to understand potential inequalities in outage management to improve and provide equal power outage reliability and services. 

The number of rows in the original DataFrame is 1534 and has 57 columns. However, the initial key variables in this analysis include electricty costs *(RES.PRICE & COM.PRICE),* urban/rural population characteristics *(POPPCT_URBAN, POPDEN_RURAL),* and outage metrics *(OUTAGE.DURATION, CUSTOMERS.AFFECTED).*

| Column Name                  | Description                                                                         |
|------------------------------|-------------------------------------------------------------------------------------|
| `'YEAR'`                     | Indicates the year when the outage event occurred                                                            |
| `'MONTH'`                    | Indicates the month when the outage event occurred                                                           |
| `'U.S._STATE'`               | Represents all the states in the continental U.S.                                                       |
| `'OUTAGE.START.DATE'`        | Indicates the day of the year when the outage event started                                       |
| `'OUTAGE.START.TIME'`        | Indicates the time of the day when the outage event started                                       |
| `'OUTAGE.RESTORATION.DATE'`  | Indicates the day of the year when power was restored to all the customers                            |
| `'OUTAGE.RESTORATION.TIME'`  | Indicates the time of the day when power was restored to all the customers                            |
| `'CAUSE.CATEGORY'`           | Categories of all the events causing the major power outages |
| `'OUTAGE.DURATION'`          | Duration of outage events (in minutes)                                              |
| `'CUSTOMERS.AFFECTED'`       | Number of customers affected by the power outage event                                   |
| `'RES.PRICE'`                | Monthly electricity price in the residential sector (cents/kilowatt-hour)                           |
| `'COM.PRICE'`                | Monthly electricity price in the commercial sector (cents/kilowatt-hour)                            |
| `'TOTAL.PRICE'`              | Average monthly electricity price in the U.S. state (cents/kilowatt-hour)          |
| `'TOTAL.SALES'`              | Total electricity consumption in the U.S. state (megawatt-hour)                    |
| `'TOTAL.CUSTOMERS'`          | Annual number of total customers served in the U.S. state                         |
| `'POPPCT_URBAN'`             | Percentage of the total population of the U.S. state represented by the urban population (in %)                           |
| `'POPDEN_RURAL'`             | Population density of the rural areas (persons per square mile)                       |
| `'NERC.REGION'`              | North American Electric Reliability Corporation (NERC) regions involved in the outage event |

# Data Cleaning and Exploratory Data Analysis 
#### Cleaning
This step begins with cleaning the data appropriately.

#### Imputation
We impute missing values.

#### Univariate Analysis
Next, we perform univariate analysis by looking at the distributions of relevant columns separately.

#### Bivariate Analysis
After this, we perform bivariate analysis. We look at the statistics of pairs of columns to identify possible associations.

#### Aggregating
We choose columns to group and pivot by in this step to examine aggregate statistics.

# Framing a Prediction Problem
#### Problem Identification
Identify a prediction problem.

# Baseline Model
#### Baseline Model
Train a “baseline model” for your prediction task that uses at least two features.

# Final Model
#### Final Model
Created a “final” model that improves upon the “baseline” model