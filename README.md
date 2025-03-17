# Vancouver Parking Tickets - Data Analysis

## Overview
This project analyzes parking ticket data in Vancouver to identify trends, high-infraction areas, and statistical differences over time. By leveraging data science techniques, we examine the relationship between parking violations and location, year, and seasonality. The goal is to extract meaningful insights that can inform urban planning and parking policy improvements.

## Data Sources
* **Primary Dataset:** Vancouver parking ticket records (2017-2024) obtained from the Vancouver Open Data Portal.
* **Supplementary Dataset:** Vancouver neighborhood boundary data used to map infractions to specific areas.
* **Geocoding API:** Google Maps API for converting street names and block numbers into latitude and longitude coordinates.

## Key Objectives
1. **Spatial Analysis:** Identify high-infraction areas using geospatial data.
2. **Temporal Trends:** Analyze year-over-year changes in parking violations.
3. **Statistical Testing:** Use ANOVA and Post Hoc analysis to determine if ticket distribution varies significantly across years.
4. **Clustering and Hotspot Detection:** Apply DBSCAN clustering to locate persistent high-infraction areas.
5. **Data Visualization:** Use heatmaps and geospatial plotting to illustrate findings.

## Methodology
1. **Data Preparation & Cleaning**
   * Filtered dataset to focus on key bylaw infractions (Bylaw 2952 and 2849).
   * Standardized and formatted data for consistency.
   * Performed a spatial join between parking ticket data and neighborhood boundaries.
   * Extracted timestamps to classify violations by quarter (Q1-Q4).
   * Handled missing and erroneous geolocation data.

2. **Geospatial Analysis**
   * Used Google Maps API to convert street-based ticket locations into latitude/longitude.
   * Conducted a spatial join to assign tickets to specific Vancouver neighborhoods.
   * Created yearly heatmaps to visualize high-infraction areas.

3. **Statistical Analysis**
   * Checked normality of ticket distribution across years using `scipy.stats.normaltest`.
   * Performed ANOVA testing to identify statistical differences in ticket volume over time.
   * Conducted Post Hoc analysis to pinpoint specific years with significant variation.

4. **Clustering & Hotspot Detection**
   * Applied **DBSCAN** (Density-Based Spatial Clustering) to find persistent violation hotspots.
   * Set parameters for clustering based on infraction density and repeat occurrences.
   * Visualized results using **Folium** maps.

## Key Findings
1. **Downtown Vancouver has the highest concentration of parking tickets.**
2. **2020 saw a statistically significant drop in violations, likely due to pandemic-related lockdowns.**
3. **Certain locations south of downtown consistently experience high infraction rates, indicating potential gaps in enforcement or signage.**
4. **Heatmaps and clustering techniques successfully identified persistent problem areas.**

## Technologies & Tools Used
* **Programming Languages:** Python
* **Libraries:** pandas, NumPy, GeoPandas, Matplotlib, Seaborn, Folium, Scipy, Statsmodels
* **APIs & Frameworks:** Google Maps API (for geocoding)
* **Statistical Analysis:** ANOVA, Post Hoc Testing
* **Clustering Algorithm:** DBSCAN
* **Version Control:** Git

## Limitations & Future Work
* The dataset lacks parking ticket pricing information, limiting deeper economic analysis.
* Additional variables (e.g., weather conditions, special events) could improve model accuracy.
* Future work could integrate predictive modeling to forecast infraction trends.

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

## Data Source
- The data source for this project is the City of Vancouver's Open Data Portal. The dataset we will be using is the Parking Ticket Data from 2018 to 2023. Link: opendata.vancouver.ca/explore/dataset/parking-tickets/information/

## Project Setup
- Clone the repository to your local machine

## Instructions
1. Extract the compressed zip folders in the data folder and drag the .csv files into the data folder
2. Ensure that geo-locations.csv, local-area-boundary.csv, parking-tickets.csv, and parking-tickets-2017-2019.csv are all in the data folder and not in any other 
3. Run the data-analysis.ipynb file through juypiter notebook or vs code and see the individual results
4. Add your Google API key 
