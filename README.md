# Public Transport queries

Query public transport connections for set of trip requests from origin to destination at given departure time. 

> This python library uses OpenTripPlanner to query single or multiple trips (origin, destination, departure time) for their detailed PT connection. 
>
> It was succesfully applied to query 3 million trips from 6 cities in the research project.

![vis](vis.png)
 
 fig.1 Sample query in Amsterdam
 
 ![vis](in.png)
 
 fig. 2 Input
 
 ![vis](out.png)
 
 fig.3 Output



### Input:
 * .csv file with requests 
 * .dbf file with OSM network (available e.g. [here](https://www.interline.io/osm/extracts/))
 * .zip with GTFS file for the area and date that we query (available e.g. from [transit.land](https://www.transit.land/)
 * both OSM and GTFS file shall be stored in `data` folder
 
 ### Output:
 * .csv with trip details
 
 
 ### Usage:
 * single trips and visualization in this tutorial [notebook](tutorial.ipynb)
 * running the OTP server [notebook](run_OTP_server.ipynb)
 * bulk queries: `python main.py`
 
