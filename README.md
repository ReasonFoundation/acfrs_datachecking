# US Municipal Financial Reports data integrity checking. Comparing with Census and National Center for Education Statistics NCES.

## Matching Census Population with Municipal Financial Reports data (ACFRs) at County Level

### Results 
Three csv files: 
* The matched dataset: `county_pop_census_acfrs_TOTAL.csv`
* counties in Census with more than 100k population that are not yet matched with ACFRs: `census_pop_NOT_match_acfrs_100k.csv`
* counties in Census, regardless of population size, that are not yet matched with ACFRs: `census_pop_NOT_match_acfrs_all.csv`

### How to just run this analysis on your machine (without cloning the whole repo)
* get the script named `acfrs_census_matching_county_population.Rmd`

* get the data object `data_from_dbsite.RDS`
This ACFRs data was queried from ACFRs PostgresQL database. The dataset was saved to R object `data_from_dbsite.RDS`. 
For security reason, the query commands are not included here.  

* get the Census Population named `DECENNIALPL2020.P1_data_with_overlays_2021-12-16T123049.csv`.
This data is located in `data` folder in the repo. 

Alternatively, this dataset can be downloaded from Census website
https://data.census.gov/cedsci/table?q=&y=2020&d=DEC%20Redistricting%20Data%20%28PL%2094-171%29&tid=DECENNIALPL2020.P1

* If you just want to push a button and not changing any directory to the data file: on your machine, create a R project -> create a folder called "data" -> Put the Census population data to that folder. 
* That's it!

## Matching Data from National Center for Education Statistics with Municipal Financial Reports data (ACFRs) at School District Level 


