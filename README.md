# Buffalo-Crime-Analysis
Buffalo city crime data analysis using matlibplot 

Crime analysis is a methodical approach for identifying and analyzing patterns and trends in crime. Crime data analysis can help the Law enforcement officers to speed up
the process of solving crimes. In this project we took the buffalo city crime data dataset and analyzed it

This dataset contains data related to the types of crime committed, time at which the crime occurred the location related information along with the police districts.
The data set has been downloaded from the state government website.
https://data.buffalony.gov/Public-Safety/Crime-Incidents/d6g9-xbgu

While analyzing we had these four important questions to answer
1. How has the crime rate changed overtime?
2. What kind of crimes occur most frequently?
3. When and where do these crimes occur?
4. Which police district has the highest crime rate?

The original dataset had close 26 features and 277k records. One of the first things we checked is for the completeness of the records and how to handle missing values, so we
decided to eliminate columns which weren’t useful for our analysis.

We normalized the data by creating two tables Incident_type and Incident table.Few columns had some values capitalized so we standardized the data before inserting
into the tables.
We also introduced a new column called Year by extracting it from the Incident_datetime column in our dataset.

The incident_type is the parent table and Incident is the child table which references the parent table using the key Incident_type_primary.
