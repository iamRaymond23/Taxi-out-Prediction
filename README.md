# TAXI-OUT PREDICTION FOR BETTER OPTIMIZING FLIGHT COSTS
Aircraft traffic operations are the major source of fuel burn and emission on the ground. Given rising fuel prices and growing concerns about the contribution of aviation to air pollution and green gas emission, this project develops a strategy to reduce fuel burn and taxi out delays at the airport.

## Business Goal
To test several models to predict taxi out of JFK airport and use the predicted results to help cut the consumption of fuel and reduce the taxi out delay.

## COMPLICATION
Understanding taxi operations and factors that affect taxi-out time.

## DATASET 
### Description of the columns
There are 28820 observations of 23 variables.
Each observation is an individual flight.
- `MONTH`, `DAY_OF_MONTH`, `DAY_OF_WEEK` contain information about the date of the flight
- `OP_UNIQUE_CARRIER` contains the ID of the airline (i.e. `AA` stands for American Airlines)
- `TAIL_NUM` is the tail number of the plane
- `DEST` is the destination airport code
- `DEP_DELAY` is the departure delay of the flight
- `CRS_ELAPSED_TIME` is the expected duration of the light
- `DISTANCE` is the distance between airports
- `CRS_DEP_M` is the scheduled departure time (in minutes after midnight)
- `DEP_TIME_M` is the actual departure time (gate checkout)
- `CRS_ARR_M` is the scheduled arrival time
- `Temperature`, `Dew Point`, `Humidity`, `Wind Speed`, `Wind Gust` and `Pressure` are the numeric characteristic of the weather
- `Wind` is the direction of the wind (`CALM` if calm, `VAR` if the wind blows from various directions)
- `Condition` contains a natural language description of the weather
- `sch_dep` is the number of flights scheduled for departure
- `sch_arr` is the number of flights scheduled for arrival 
- `TAXI_OUT` is the time between the actual pushback and wheels-off.

There are five categorical variables: `OP_UNIQUE_CARRIER`, `TAIL_NUM`, `DEST`, `WIND` and `Condition`. 
The rest of the variables are numerical.
Our target variable is `TAXI_OUT`.
