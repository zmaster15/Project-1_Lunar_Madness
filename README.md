<h1 align = "center" > Lunar Lunacy Effect </h1>
<h3 align = "center" > Fact or Fiction? </h3>
<p align = "center" >
    <img title="Lunar Madness" img src = "lunar_madness.png" alt = "Lunar Madness" width = "300"/>
    </p>

## Executive Summary:  
The Lunar Madness team investigated correlations between full moon and crime statistics in four diverse US cities. The main objective is to investigate publicly available crime data and known moon phase  data.  If correlations can be established then opportunities to contract and assist, help further investigate local data and staffing history for clients such as municipalities, local government, law enforcement, hospitals, and first responders of established patterns to assist them in planning for staffing needs and preparedness based on future research. 
- Revised RS ~ How about Below ? --  Expand on this (Sheila/Raymond) - look for similar projects with comparison, open source, add monetary pitch
The Lunar Madness project analyzes potential correlations between full moons and crime rates in four U.S. cities. Its goal is to leverage public crime statistics and lunar phase data to identify patterns that could help organizations optimize staffing and resource allocation. Target clients include local governments, law enforcement agencies, hospitals, and first responders who could benefit from predictive scheduling based on lunar-correlated incident patterns.

## Table of Contents
- [Lunar Lunacy Project Overview]
 ~ RS> README file includes a concise project overview 
 ~ RS> Definition (Format with indention) (#lunar-lunacy-effect-defined)
 ~ RS> Project scope
 ~ RS> [Hypothesis](#hypothesis)
 ~ RS> GitHub README file includes detailed usage and installation instructions 
      ~ Requirements (Tech stuff - Minimum requirements (Python 3.16 or greater, Jupyer notebooks, Import Dependancies (list: Pandas, plotly, etc.))

Data Preparation and Analysys
    - [Identify Correlation](#identify-correlation)
    - [Statistical Significance](#statistical-significance)
    - [Staffing Needs](#staffing-needs)
- [Conclusion] (#conclusion)
    - [Findings] (#findings)
    - [Lessons Learned] (#lessons learned)
    - [Next Steps - Recommendations for the future] (#next steps)  
- [Appendix] 
    - [Data Sources](#data-sources)
    - [Team Members](#team-members)


## Lunar Lunacy Effect Defined
# RS~ Summerize down to ?:   
The idea that the full moon influences human behavior, sometimes called the "lunar lunacy effect" or "Transylvania effect," has been around for centuries. The term "lunatic" even originates from the Latin word *luna*, meaning "moon." Throughout history, folklore and myths from around the world have associated the full moon to erratic behavior, ranging from medieval legends of werewolves and vampires to more modern theories suggesting that the moon's gravitational pull might affect the brain's fluids and, in turn, behavior. 

## Hypothesis
The Lunar Madness team sought to test the validity of the lunar lunacy effect by comparing crime and traffic data against full moon dates in 4 major metropolitan cities: Austin, Denver, Houston and Los Angeles. If our hypothesis is true, we should see a higher volume of erratic behavior on days with a full moon. Add details on null hypothesis, etc.

Erratic behavior is defined as "unpredictable, irregular, or inconsistent behavior that deviates from what is considered normal. It wan include mood swings, impulsive actions, and exaggerated emotional responses. 


## Identify Correlation:
We will investigate and look for patterns that indicate if people’s criminal behavior are influenced by the lunar cycle. Explore potential explanations for any observed correlations (e.g., increased visibility during full moon).

Questions to be answered: Rework
1. Is there is a strong correlation between the full moon and crime is cities?

3. If these effects exist, drill down and identify more granular relationships in the data
4. Explore other relationships that may be uncovered during the initial exploratory analysis
Identify if there is a strong correlation between full moon and traffic accidents
5. If the disparate city crime data can be categorized with specific crime types,


## Statistical Significance:
- Determine if there is a statistically significant correlation between moon phases and crime rates in sampled metropolitan areas (Chicago, Austin, Denver & Los Angels).

- Identify any specific crime types that may be more strongly influenced by the lunar cycle. Explore potential explanations for any observed correlations (e.g., increased visibility during full moon).

## Analysis 
- (aggregation, correlation, comparison, summary statistics, and *time series analysis*)
- intake data
- normalize it
- merge moon and city crime data
- analyze data
- visualize data
- summarize
- Zain: To understand what data we have and what can we do with it. 
Read in the moon data files, pulling out the phases of the moon and the date
Convert date column to datetime
Explain Phases, other
Read in the cleaned crime data, convert date column to datetime (had issues converting to datetime with UTC time, so learned had to use .dt.date to remove first, then )
![alt text](image.png)
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

## Staffing Needs:
If proven that there is high correlation between crime related offenses with the phases of the moon, this information could then be useful for properly staffing respective public departments (law enforcement, tow trucks, emergency services, Fire Stations, hospitals, and 911 call centers) to support a higher volume of erratic behavior.

## Findings: 


## Lessons Learned
GitHub - have .ignore file, 
Version control
Look at each phase of the moon to see if there was statistical signoficance
Communication - did not define roles initially, ended up with multiple 

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
