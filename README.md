# ETL-Project-Spar-Nord-Bank

![image](images/atm.avif)

## About this project

**Spar Nord Bank** is trying to observe the withdrawal behavior and the corresponding dependent factors to optimally manage the refill frequency. Apart from this, other insights also have to be drawn from the data.

Spar Nord Bank has data from more than 100 ATMs across DenMark. Data is captured every transaction including withdrawn amount, card type, location, date, time, ATM type, etc.

Spar Nord Bank need to build a Dimensional Model datastore (ATM Data Mart) on this ATM transaction data to understand the ATM usage pattern.

## Tasks

Build a batch ETL pipeline to read transactions data from RDS, transform and load data into target dimensions and facts on Redshift Data Mart.

Once data is loaded in Redshift, write analytical queries to answer business questions:

- Top 10 ATMs where most transactions are in the ’inactive’ state

- Number of ATM failures corresponding to the different weather conditions recorded at the time of the transactions

- Top 10 ATMs with the most number of transactions throughout the year

- Number of overall ATM transactions going inactive per month for each month

- Top 10 ATMs with the highest total amount withdrawn throughout the year

- Number of failed ATM transactions across various card types

- Top 10 records with the number of transactions ordered by the ATM_number, ATM_manufacturer, location, weekend_flag and then total_transaction_count, on weekdays and on weekends throughout the year

- Most active day in each ATMs from location "Vejgaard"
