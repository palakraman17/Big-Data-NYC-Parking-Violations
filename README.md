# Big Data NYC Parking Violations

These scripts analyze different aspects of parking violations in NYC using both Hadoop Streaming and Spark.

## Data 

The data used is open and available from NYC Open Data:
* Parking Violations Issued (Fiscal Year 2016) https://data.cityofnewyork.us/City-Government/Parking-Violations-Issued-Fiscal-Year-2016/kiv2-tbus/data
* Open Parking and Camera Violations https://data.cityofnewyork.us/City-Government/Open-Parking-and-Camera-Violations/nc67-uf89

## Tasks

1. Write a Map Reduce(using 2 reducers) job, Spark and SparkSQL programs to find all parking violations that have been paid, i.e., that do not occur in open-violations.csv. 
2. Write a Map Reduce(using 2 reducers) job, Spark and SparkSQL programs to find the frequencies of the violation types in parking_violations.csv, i.e., for each violation code, the number of violations that this code has.
3. Write a Map Reduce(using 2 reducers) job, Spark and SparkSQL programs to find the total and average amounts due in open violations for each license type.
4. Write Spark and SparkSQL programs to compute the total number of violations for vehicles registered in the state of NY and all other vehicles.
5. Write Spark and SparkSQL programs to find the vehicle that has had the greatest number of violations (assume that plate_id and registration_state uniquely identify a vehicle).
6. Write Spark and SparkSQL programs to find the top-20 vehicles in terms of total violations (assume that plate_id and registration_state uniquely identify a vehicle).
7.  Write Spark and SparkSQL programs that for each violation code, list the average number of violations with that code issued per day on weekdays and weekend days. You may hardcode “8” as the number of weekend days and “23” as the number of weekdays in March 2016. In March 2016, the 5th, 6th, 12th, 13th, 19th, 20th, 26th, and 27th were weekend days (i.e., Sat. and Sun.)
