# Data Modelling with Apache Cassandra
A startup called Sparkify wants to analyze the data they've been collecting on songs and user activity on their new music streaming app. The analysis team is particularly interested in understanding what songs users are listening to. Currently, there is no easy way to query the data to generate the results, since the data reside in a directory of CSV files on user activity on the app.
In this project, I am taking on the role of a data engineer at Sparkify tasked with tackling a crucial aspect of Sparkify's music streaming service: understanding user listening habits. By building an Apache Cassandra database, we can efficiently analyze songplay data and answer key questions about user preferences. The project involved designing data models within Cassandra to enable powerful queries focused on popular songs and listening trends. Additionally, an ETL pipeline was created to streamline data processing, ensuring smooth data flow and analysis for Sparkify's music recommendation engine.
Specifically, the data modelling tasks are centered around three questions:

### Give me the artist, song title and song's length in the music app history that was heard > during sessionId = 338, and itemInSession = 4
### Give me only the following: name of artist, song (sorted by itemInSession) and user (first and last name) for userid = 10, sessionid = 182
### Give me every user name (first and last) in my music app history who listened to the song 'All Hands Against His Own'

## Project Steps
Below are steps were followed to complete each component of this project.

### Modeling your NoSQL database or Apache Cassandra database
1. Design tables to answer the queries outlined in the project template
2. Write Apache Cassandra CREATE KEYSPACE and SET KEYSPACE statements
3. Develop your CREATE statement for each of the tables to address each question
4. Load the data with INSERT statement for each of the tables
5. Include IF NOT EXISTS clauses in your CREATE statements to create tables only if the tables do not already exist. We   
   recommend you also include DROP TABLE statement for each table, this way you can run drop and create tables whenever you 
   want to reset your database and test your ETL pipeline
6. Test by running the proper select statements with the correct WHERE clause

### Build ETL Pipeline
1. Implement the logic in section Part I of the notebook template to iterate through each event file in event_data to 
   process and create a new CSV file in Python
2. Make necessary edits to Part II of the notebook template to include Apache Cassandra CREATE and INSERT statements to load 
   processed records into relevant tables in your data model
3. Test by running SELECT statements after running the queries on your database

## Prerequisites
1. cassandra
2. pandas
3. csv
4. os
5. numpy
6. Jupyter notebook and python 3 are needed to run the notebooks and python scripts. For ease, consider installing ANACONDA.

## Instructions on running the application
Download the required data sets and modify the directory paths. Along with this, you are also required to have a running instance of Apache Cassandra installed on your device. Lastly, follow the instructions provided in the Jupyter notebook to perform ETL and build the data pipeline.
