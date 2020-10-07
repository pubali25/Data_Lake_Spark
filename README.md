*Project*: Data Lake

**Introduction**
A music streaming startup, Sparkify, has grown their user base and song database even more and want to move their data warehouse to a data lake. Their data resides in S3, in a directory of JSON logs on user activity on the app, as well as a directory with JSON metadata on the songs in their app.

As their data engineer, I am asked with building an ETL pipeline that extracts their data from S3, processes them using Spark, and loads the data back into S3 as a set of dimensional tables. This will allow their analytics team to continue finding insights in what songs their users are listening to.



**Project Description**
In this project, I have to load data from S3, process the data into analytics tables using Spark, and load them back into S3. You'll deploy this Spark process on a cluster using AWS.

Schema for Song Play Analysis
Using the song and log datasets, I'll need to create a star schema optimized for queries on song play analysis. This includes the following tables.

**Fact Table**

songplays - records in log data associated with song plays i.e. records with page NextSong
songplay_id, start_time, user_id, level, song_id, artist_id, session_id, location, user_agent

**Dimension Tables**
users - users in the app
user_id, first_name, last_name, gender, level
songs - songs in music database
song_id, title, artist_id, year, duration
artists - artists in music database
artist_id, name, location, lattitude, longitude
time - timestamps of records in songplays broken down into specific units
start_time, hour, day, week, month, year, weekday


**Project Datasets**

Song data: s3://udacity-dend/song_data
Log data: s3://udacity-dend/log_data

**Steps of the Project**
1.Load Data from S3
2.Process the data with Spark
3.Load it back to S3

