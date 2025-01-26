<h1 align = "center" > Lunar Lunacy Effect </h1>
<h3 align = "center" > Fact or Fiction? </h3>
<p align = "center" >
    <img title="Lunar Madness" img src = "lunar_madness.png" alt = "Lunar Madness" width = "300"/>
    </p>

## Executive Summary  
The Lunar Madness project analyzes potential correlations between full moons and crime rates in four U.S. cities. Its goal is to leverage public crime statistics and lunar phase data to identify patterns that could help organizations optimize staffing and resource allocation. Target clients include local governments, law enforcement agencies, hospitals, and first responders who could benefit from predictive scheduling based on lunar-correlated incident patterns. 

## Table of Contents
[Lunar Madness Project Overview](#lunar-madness-project-overview)  
- [Project Requirements](project-requirements)  
- [Data Collection](#data-collection)  
- [Data Analysis](#data-analysis)
- [Identify Correlation](#identify-correlation)
- [Statistical Significance](#statistical-significance)
[Conclusion](#conclusion)
    - [Lessons Learned](#lessons-learned)
    - [Next Steps](#next steps)  
- [Appendix] 
    - [Data Sources](#data-sources)
    - [Team Members](#team-members)


## Lunar Madness Project Overview
The Lunar Madness project aims to prove the urban legend that the full moon causes erratic behavior by comparing moon phase data against reported crime and traffic data for multiple major metropolitan cities. 

If proven that there is high correlation between crime-related offenses with the phases of the moon, this information could then be used to ensure appropriate staffing levels for respective public departments (law enforcement, tow trucks, emergency services, Fire Stations, hospitals, and 911 call centers) to support a higher volume of erratic behavior.

## Project Requirements   
[Python 3.16 or greater](https://www.python.org/)   
[Jupyter Notebook](https://jupyter.org/)  
GitHub Repository   
Import Dependancies: Pandas, plotly, datetime

## Data Collection: See [Data Sources](#data-sources)  
- intake data
- normalize it
- merge moon and city crime data
1. Moon phase data collected from the U.S. Naval Observatory and the National Weather Service.  
    - Initial assessment conducted to understand the data and identify any issues
        - Read in each year from 2013-2024 and convert to a new DataFrame
        - Combined into Moon Phase DataFrame to be used for analysis 
        ![moon_data_export](Resources\combined_moon_data.png)
2. Crime data cleaned and normalized for the following cities:  
    - Austin  
    - Chicago  
    - Denver   
    - Houston  
    - Los Angeles  
3. Merged moon data with the crime data for each city

## Data Analysis:
- Determine if there is a statistically significant correlation between moon phases and crime rates in sampled metropolitan areas (Chicago, Austin, Denver & Los Angels).
- Identify any specific crime types that may be more strongly influenced by the lunar cycle. Explore potential explanations for any observed correlations (e.g., increased visibility during full moon).
- (aggregation, correlation, comparison, summary statistics, and *time series analysis*)

- analyze data
- visualize data
- summarize

Merge data sets: Merged on Date using pd.merge right join, filled blank dates with other
Aggregated total count of offenses that occurred on each date
![alt text](image-1.png)
Plot of Los Angeles Crime Data by Day
Sliced data for 2020-2024
![alt text](image-2.png)

Outlier crime data: 
![alt text](image-3.png)
![alt text](image-4.png)
![Full Moon Normalized](image-5.png)
No pattern identified
![alt text](image-6.png)
![alt text](image-7.png)
Traffic ![alt text](image-8.png)
![alt text](image-9.png)
![alt text](image-10.png)

## Conclusion:


## Lessons Learned:
had issues converting to datetime with UTC time, so learned how to use .dt.date to remove first, then )
![alt text](image.png)
GitHub - have .ignore file, 
Version control
Look at each phase of the moon to see if there was statistical signoficance
Communication - did not define roles initially, ended up with multiple data files causing confusion in Analysis

## Next Steps:



## Data Sources:
### Full Moon Data Sources:
- [National Weather Service](https://www.weather.gov/box/sunmoon)
 (National Oceanic and Atmospheric Administration)  
Data Points:  Daily moon phase information (e.g., new moon, full moon, first quarter, last quarter, percentage of illumination)  

- [US Naval Observatory Moon Phases](https://aa.usno.navy.mil/calculated/moon/phases?date=2024-01-10&nump=50&format=t&submit=Get+Data)  
Data Points:  Daily moon phase information (e.g., new moon, full moon, first quarter, last quarter)   

### Crime Data Sources:
- [US Government provided data](https://catalog.data.gov/dataset/?tags=crime)  
Data Points: Date and time of each reported crime incident, Crime type  

- [Los Angeles Crime Data](https://data.lacity.org/Public-Safety/Crime-Data-from-2020-to-Present/2nrs-mtv8/about_data)  
Data Points: Date and time of each reported crime incident, Crime type  

- [Houston Crime Data](https://www.kaggle.com/datasets/iamkevin/raw-aggregate-houston-crime-report-data)  
Data Points: Date and time of each reported crime incident, Crime type  

- [Denver Crime Data](https://www.kaggle.com/code/paulo098/denver-crime-data-analysis-and-prediction)  
Data Points: Date and time of each reported crime incident, Crime type  

- [Austin Crime Data](https://catalog.data.gov/dataset/crime-reports-bf2b7)  
Data Points: Date and time of each reported crime incident, Crime type  

### Traffic Data Source
- [Maryland Traffic Data](https://data.montgomerycountymd.gov/Public-Safety/Traffic-Violations/4mse-ku6q/about_data)


## Team Members: (add images)
Data Engineer: Sheila Mathews  
Data Analyst: Raymond Stover  
Data Scientist: Michael Brady  
Data Scientist: Zain Master  

## [Presentation](https://docs.google.com/presentation/d/1stl1fJb9OlSzICY6XXBW35ircUMwCN8yHXWsC-sYAcs/edit?usp=sharing)
