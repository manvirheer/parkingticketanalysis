# CMPT 353 Group Project - Parking Ticket Analysis in City of Vancouver
## Group Members
- [Manvir Singh Heer](https://github.sfu.ca/msh16)
- [Kevin Chung](https://github.sfu.ca/klc30)

## Collaboration Rules
- Work on dev branch only and create a pull request to merge with main branch
- Use the following format for commit messages: 
  - `git commit -m "chore: description"` for general additions or changes
  - `git commit -m "bug: description"` for bug fixes
  - `git commit -m "docs: description"` for documentation changes
- Update README.md with any changes made to the project

## Project Description
- This project is a computational data science project where we will be analyzing the geographic and temporal trends in parking ticekts issued in City of Vancouver.

## Data Source
- The data source for this project is the City of Vancouver's Open Data Portal. The dataset we will be using is the Parking Ticket Data from 2018 to 2023. Link: opendata.vancouver.ca/explore/dataset/parking-tickets/information/
- The other data set is 


## Project Setup
- Clone the repository to your local machine
- Download 

## Instructions
1. Extract the compressed zip folders in the data folder and drag the .csv files into the data folder
2. Ensure that geo-locations.csv, local-area-boundary.csv, parking-tickets.csv, and parking-tickets-2017-2019.csv are all in the data folder and not in any other 
3. Run the data-analysis.ipynb file through juypiter notebook or vs code and see the individual results 

## Project Plan
- The project will be divided into the following phases:
  - Data Collection
    - Work on collecting the data from the City of Vancouver's Open Data Portal **(Manvir)**
    - Work with Google Maps API to get the geoencoding of the addresses in the dataset **(Manvir & Kevin)**
  - Data Cleaning, Filtering, Formatting
    - Change the dates to a standard format of separate columns for year, month, day, time **(Manvir)**
    - Add the geoencoding to the dataset **(Manvir)**
    - Add the quarter of the year to the dataset **(Kevin)**
  - Data Analysis
    - General analysis of the data to do exploratory data analysis
    - Analysis of the data to find the most ticketed areas in the city
    - Analysis of the data to find the most ticketed times in the city
    - Analysis of temporal trends in the data
    - Analysis of geographic trends in the data
    
  - Data Visualization
    - Based on previous analysis, create visualizations to represent the data
  
  - Report Writing
    - Write a report on the findings of the analysis and visualization
