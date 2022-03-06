# PROJECT: vinif_bus_time_tables
The central aim of the project is to develope a Timetables for Bus System in HCMC (Saigon South), Vietnam. This project is supported in part by Vingroup Innovation Foundation, Vietnam. 

Main tasks
==========
1. Discover the bus top sequences of bus lines using bus stop information (long-lat) and historical bus locations  
2. Calculate distance ratio & arrival time at each bus stop along the path
3. Calculate (Interpolate) Arrive Time for each Stops
4. Calculate Timetables for the Bus System 

Input Data
==========
Data was requested from Busmap Vietnam, including:'routes.json', 'timetables.json', 'trips.json', 'vars.json', 'paths.json', 'stops.json'
Data problems:
1. Data only contains bus stops location (i.e. longitude, latitude) and bus route numbers in each stop. There is no bus route
2. Available data from Jan 2019 - Sep 2019 
3. The data recording the distance traveled by the bus had a lot of noise, e.g. the distance increases and decreases continuously
4. We don't know how many times the bus runs a day
5. The departure time (first departure) of each trip is unknown, and the time when the bus arrives at the final station (the last stop on the route) is unknown as well
6. There are cases where the bus has reached the last station but the data is still recorded (same location, data is recorded continuously and repeatedly) so it is necessary to determine when the bus actually arrives at the last station
