Data Modeling with Postgres
-----------------------------
Sparkify is a startup, they want to analyze the data and they have been collecting songs and user activity on their new music streaming app. There is an analysis particularly interested in understanding what songs users listen to. They do not have any easy method to query their data, which resides in a JSON log directory of user activity on the app, as well as a directory with JSON metadata about the Songs app.

Data engineers to create a Postgres database of tables that streamline Song play analytic queries and lead them to the project. There is a job to create the database schema and ETL pipeline for this analysis. Database testing and ETL pipeline by running queries from the Sparkify analytics team and comparing the results to the expected results.
Describe project
----------------
In this project, I will apply what I have learned about data modeling with Postgres and build an ETL pipeline in Python. To complete the project, I will need to define a fact table and dimensions for the figure schema for a specific analysis purpose, and write an ETL pipeline that converts the data from files in two local directories to Postgres in Python and SQL. Convert these tables with Python and SQL

Requirements
------------

Python 3 is available
pandas and psycopg2 are available
A PosgreSQL database is available on 

Run a python script
-------------------
At the terminal:

python create_tables.py
python etl.py
In IPython:

run create_tables.py
run etl.py

ETL Process
-----------
The first dataset is a subset of the actual data in the Million Song dataset. Every file are in JSON format and metadata contain about songs and artist's songs.The file is split according to the first three letters of the track ID for each song. For example, the file paths to the two files in this dataset are:

song_data/A/B/C/TRABCEI128F424C983.json
song_data/A/A/B/TRAABJL12903CDCF1A.json

Description of Files
--------------------

data/log_data:

These files are used to populate the Song Plays fact table  and  the User and Time dimension tables.

data/song_data:

These files are used to fill the dimension table for songs and artists

create_tables.py :- 

This Python script rebuilds the database and tables used to store the data.

etl.ipynb :-

The Python Jupyter notebook was originally used to track data and test the ETL process.

etl.py :-

I first examined the data and tested the ETL process using a Python Jupyter notebook.
 
sql_queries.py:-

A Python script that defines all the SQL statements used in this project.

test.ipynb:- 
The Python Jupyter notebook used to test that the data was loaded correctly.











 

