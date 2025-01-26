# Public Transport Timetable Prediction  

The primary objective of this project is to develop timetables for the bus system in Ho Chi Minh City (Saigon South), Vietnam. This project is partially funded by the Vingroup Innovation Foundation, Vietnam.  

## Main Tasks  

1. Identify the sequences of bus stops for each bus route using bus stop location data (longitude and latitude) and historical bus location data.  
2. Calculate the distance ratio and arrival time at each bus stop along the route.  
3. Interpolate and calculate the arrival time for each bus stop.  
4. Generate timetables for the entire bus system.  

## Input Data and Data Quality  

### **Input Data**  

The data was obtained from Busmap Vietnam and includes the following files:  
- `routes.json`  
- `timetables.json`  
- `trips.json`  
- `vars.json`  
- `paths.json`  
- `stops.json`  

### **Data Issues**  

1. The data only contains bus stop locations (longitude and latitude) and the bus route numbers for each stop, but not the full route details.  
2. The available data spans the period from January 2019 to September 2019.  
3. There is significant noise in the data recording the distances travelled by buses; for example, the recorded distances frequently increase and decrease inconsistently.  
4. The number of times a bus runs each day is unknown.  
5. The departure time of the first trip for each bus and the arrival time at the final station (the last stop on the route) are both unknown.  
6. In some cases, the data shows the bus repeatedly recorded at the final station (same location, recorded continuously), making it necessary to determine when the bus actually arrives at the final station.

Result
==========
**Bus Trajectory**

<img src="fig/bus stop and bus trajectory.png" alt="Example" width="100%" />

**Number of trip / day**

<img src="fig/number of trip a day.png" alt="Example" width="100%" />

**Velocity-noise remove**
<img src="fig/velocity noise remove.png" alt="Example" width="100%" />

