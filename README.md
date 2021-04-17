# WorldNews-UpVotes-Anomaly-Detection-LSTM
1. Dataset
  A large dataset (72.7 MB) of time-series news information published on Worldnews, 

1. Motivation 

    Given a large dataset of time-series news information published on Worldnews, I want to investigate the  
    A starup company wants to analyze the data of songs and user activity on their music streaming app. 
    Song data resides in a directory with JSON metadata on the songs in their app and activity data resides 
    in a directory of JSON logs on user activity on the app.
    The company wants to create a Postgres database schema and ETL pipeline for this analysis. 
  
2. Methods

  * `create_tables.py`
    
    The script connects to the Sparkify database, drops any tables if they exist, and creates the tables
  * `sql_queries.py`
    
    The scirpt specify all columns for each of the five tables (`songplays`, `users`, `songs`, `artists`, `time`). 
    The ER diagram is shown below:
    ![ER diagram](ER.png)
  * `etl.py`
    
    The script connects to the Sparkify database, extracts and processes the `log_data` and `song_data`, and insert data into the five tables.
3. Technologies Used

 * Python
    - numpy
    - pandas
    - psycopg2
    - os
    - glob
 * PostgreSQL
 
 
4. How to run the scripts

    First run `create_tables.py`, then run `etl.py`.
