## DEND Project:  Data Modeling with Cassandra
[![N|Solid](https://i2.wp.com/blog.knoldus.com/wp-content/uploads/2018/06/screenshot-from-2018-06-04-15-06-42.png?fit=726%2C334&ssl=1)](https://www.postgresql.org)


### Project Description
A startup called Sparkify wants to analyze the data they've been collecting on songs and user activity which resides in a directory of the data reside in CSV files.

In this scenario, we acting as the data engineer on the team are to create a NoSQL Cassandra database with tables designed to optimize queries on song play analysis. We are to create a database schema and ETL pipeline for this analysis.

Files:
-- Dataset in  'P2-csv_files' - the directory of CSV files partitioned by date
-- Datafiles 'event_datafile_new.csv' dataset to create a denormalized dataset

Tasks:
- Modeled the data tables w.r.t. the CQL (NoSQL) queries we want to run
- loaded the data into tables we created in Apache Cassandra and run our queries
- Create a database schema and ETL pipeline for the analysis of these data and log files
- Test the database and ETL pipeline by running queries

##### Song Dataset
The Song dataset is a subset of real data from the Million Song Dataset. Each file is in JSON format and contains metadata about a song and the artist of that song. The files are partitioned by the first three letters of each song's track ID

##### Project Steps
Below are steps I followed to complete each component:

- Modeling the NoSQL database or Apache Cassandra database
- Designed tables to answer the queries outlined in the project
- Wrote Apache Cassandra CREATE KEYSPACE and SET KEYSPACE statements
- Developed CREATE statements for each of the tables to address each question
- Loaded the data with INSERT statement for each of the tables
- Included IF NOT EXISTS clauses in the CREATE statements to create tables - Included DROP TABLE statement for each table to reset the database and test ETL pipeline
- Tested by running the proper select statements with the correct WHERE clause

##### Build ETL Pipeline
1) Implemented the logic in section Part I of the notebook to iterate through each event file in event_data to process and create a new CSV file in Python
2) Made necessary edits to Part II of the notebook to include Apache Cassandra CREATE and INSERT statements to load processed records into relevant tables in the data model
3) Tested by running SELECT statements after running the queries on the database


-------------------------------------------------------------------------
