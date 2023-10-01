# Geoprocessing summary

## Mapping question:
How many Wind Turbines are within 100 miles of Grand Canyon National Park outter boundaries?


## Data utilized:
USGS Wind turbines - https://eerscmap.usgs.gov/uswtdb/
State boundaries - US Census Bureau - https://www.census.gov/geographies/mapping-files/time-series/geo/carto-boundary-file.html
Grand Canyon Boundary - US National Parks Service - https://public-nps.opendata.arcgis.com/datasets/nps-boundary-1/explore?location=42.102470%2C-70.956425%2C5.77


## Result: 
![Grand Canyon Map](grandCanyon1.png)

There are 194 wind turbines within 100 miles of Grand Canyon Nation Park.



## Mapping answer:
I used a Buffer to establish 100 linear miles from the outer boundaries of the national park. i then used select attributes by location to identify the wind turbines located within 100 miles of the national park and extported those selected feature to their own GEOjson. Then used a count query to get the total number of wind turbines. By doing this I was able to get the excact number of wind turbines.