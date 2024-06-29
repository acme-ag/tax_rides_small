# taxi_rides_small
Small dataset for EDA and modelling

# Features:
- id: a unique identifier for each trip
- vendor_id - a code indicating the provider associated with the trip record
- pickup_datetime - date and time when the meter was engaged
- dropoff_datetime - date and time when the meter was disengaged
- passenger_count - the number of passengers in the vehicle (driver entered value)
- pickup_longitude - the longitude where the meter was engaged
- pickup_latitude - the latitude where the meter was engaged
- dropoff_longitude - the longitude where the meter was disengaged
- dropoff_latitude - the latitude where the meter was disengaged
- store_and_fwd_flag - This flag indicates whether the trip record was held in vehicle memory before sending to the vendor because the vehicle did not have a connection to the server - Y=store and forward; N=not a store and forward trip
- trip_duration - duration of the trip in seconds

The idea is to test EDA - how much it can add - and try modelling on a limited number of variables.

Although the largest R2 score is 72% for test, - which is not bad, - the conclusion is that the dataset is small, with only about 60,000 data points and a small number of variables. Within this dataset, it is unlikely to achieve a better R^2 score — these predictors are insufficient for building a better model. It would be possible to use external datasets, such as more precise geodata or data on trip costs.
