# Lunar Madness

<h1 align = "center" > Lunar Lunacy Effect </h1>
<h3 align = "center" > Fact or Fiction? </h3>
<p align = "center" >
    <img title="Lunar Madness" img src = "Resources/lunar_madness.png" alt = "Lunar Madness" width = "300"/>
    </p>

## Executive Summary  

The **Lunar Madness** project analyzes potential correlations between full moons and crime rates in five U.S. cities. The goal is to leverage public crime statistics and known lunar data to identify patterns that could help organizations optimize staffing and resource allocations. Target clients include local governments, law enforcement agencies, hospitals, and first responders who could benefit from predictive scheduling based on lunar-correlated incident patterns.

## Table of Contents  

- [Project Overview](#project-overview)  
  - [Project Requirements](#project-requirements)  
  - [Data Collection](#data-collection)  
  - [Data Analysis](#data-analysis)
- [Conclusion](#conclusion)
  - [Statistical Significance](#statistical-significance)
  - [Lessons Learned](#lessons-learned)
  - [Next Steps](#next-steps)  
- [Data Sources](#data-sources) 
- [Team Mambers](#team-members)
- [Presentation](#presentation)

## Project Overview  
  
The Lunar Madness project Team is investigating the urban legend that correlates erratic behavior when the moon is in its Full phase. By comparing moon phase data against reported crime and traffic data for multiple major metropolitan cities, the project seeks to determine if there is a statistically significant correlation. If a strong correlation is identified, this preliminay proof of concept could be used as a basis for future investigation.  Businesses and municipalities could benefit from the investigative work of the Lunar Madness Team to help inform optimized staffing levels, fleet preparations, and advising on supply inventories for public departments such as law enforcement, emergency services, and hospitals during specific lunar phases.



## Project Requirements

- **Software Requirements:**
  - [Python 3.16 or greater](https://www.python.org/)   
  - [Jupyter Notebook](https://jupyter.org/)
  - GitHub account   
  - Load Dependancies: 
    ```
    import pandas as pd
    from prophet import Prophet
    import datetime as dt
    import numpy as np
    import matplotlib.pyplot as plt
    %matplotlib inline 
    ```
- **GitHub Repository Structure:**
``` Markdown for Clean display of GitHub Repository Structure
  📦Project-1_Lunar_Madness 
      ┣ 📂Michael (Project Notebooks and CSV working files (Austin, Denver, Chicago, LA & Moon))
      ┣ 📂Raymond (Practice & Investigative Jupyter, Notes and test files )
      ┣ 📂Shelia  (Cleand Moon Source file Jupyter Project notebooks, & export CSV) 
      ┣ 📂Zain (Jupyter Project notebooks for )
      ┣ 📂Resources (Data Source files and images for project) 
      ┣ 📜.DS_Store
      ┣ 📜.gitattributes
      ┣ 📜.gitignore
      ┣ 📜Howlers_(Lunar Madness)_Project_Sheet.xlsx
      ┣ 📜LICENSE 
      ┣ 📜README.md 
      ┗ 📜lunar_madness.png
```
## Data Collection 
- (Also See [Data Sources](#data-sources))  
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
3. Moon data merged with the crime data for each city  
Houston
![houston_moon_combined](image-1.png)

## Data Analysis:
- Determine if there is a statistically significant correlation between moon phases and crime rates in sampled metropolitan areas (Chicago, Houston, Austin, Denver & Los Angeles).
- Identify any specific crime types that may be more strongly influenced by the lunar cycle. Explore potential explanations for any observed correlations (e.g., increased visibility during full moon).
- Aggregation:  
![crime_count](Resources\crime_count.png)


, correlation, comparison, summary statistics, and *time series analysis*)


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
Obtaining Data that is accurate and reliable early on is important.  Processing data files take time and diligence to normalize as there may be time zone, UTC and formatting issues.  Communication and role assignments could have been managed better in hindsight and had we communicated roles and responsibilities with expected deliverables we would have had more focused work from the start using agreed upon standard files.  Version control and using github can be a challenge.  The .DSstore file from the Apple IOS proved to be problematic and 'dot ignore' file is mandatory at this level of programming.  Wometimes the most recent data is not comprobable and needs to be truncated.  Data can have irregularities and data needs to be normalized.  Different types of plotting reveal differt patterns within the data.




## Next Steps:


## Appendix
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
