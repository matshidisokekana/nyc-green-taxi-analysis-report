# nyc-green-taxi-analysis-report

## *Introduction*  
This Power BI project analyzes *NYC Green Taxi trips in 2023*, focusing on trip distribution across boroughs and zones. It provides insights into trip frequency, pickup and drop-off locations, and trends using interactive visualizations.  

### *Problem Statement *  

❓ *How can we identify the most popular pickup and drop-off locations for NYC Green Taxi trips?*  
✔ *By analyzing trip data, we found that Manhattan, Queens, and Brooklyn have the highest trip counts, with specific zones like Crown Heights, Astoria, and JFK Airport being key hotspots.*  

❓ *Are there imbalances between pickup and drop-off locations?*  
✔ *Yes, some zones have significantly more pickups than drop-offs (e.g., LocationID 41 with 1.3M pickups but only 898K drop-offs). This suggests areas where passengers frequently start their trips but do not return via taxi.*  

❓ *Which boroughs and zones have the lowest trip volumes, and why?*  
✔ *Staten Island, EWR (Newark Airport), and unknown zones have the lowest trip counts. This could be due to limited Green Taxi availability, lower demand, or alternative transport options in these areas.*  

❓ *How well is the taxi service distributed across different boroughs?*  
✔ *Drop-offs are evenly distributed across boroughs (each contributing about 12.5%), but pickup hotspots suggest that taxis are more concentrated in central NYC.* 

## *Skills Demonstrated*  
- *Data Sourcing & Transformation* (Azure Databricks, Power BI)  
- *Data Modeling* (Relational data connections)  
- *Data Visualization* (Charts, tables, and maps for insights)  
- *Power BI DAX & Measures* (Aggregations and calculations)
   
## *Data Sourcing*  
The dataset is sourced from *Azure Databricks*, containing records on Green Taxi trips in NYC, including:  
- *Trip locations* (Pickup & Drop-off Location IDs)  
- *Borough & Zone mapping*  
- *Taxi type classification*

#### *Transformations Applied:*  
1. *Filtering the Top 10 Locations:*  
   - The dataset originally contained a large number of unique pickup and drop-off locations.  
   - Applied a *Top 10 filter* on *PULocationID and DOLocationID* based on trip counts.  
   - This helps in focusing on the most significant zones for analysis.  

2. *Aggregation of Trip Counts:*  
   - Calculated the *total number of trips* per pickup and drop-off location.  
   - Ranked them to identify the *most frequently used locations*.  

3. *Reducing Data Volume for Performance Optimization:*  
   - Limiting data to the *top 10 locations* ensures better visualization performance.  
   - Reduces clutter in the reports, making insights more actionable.











