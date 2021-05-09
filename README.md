The README file includes a summary of the project, how to run the Python scripts, and an explanation of the files in the repository.


NOTE: You will not be able to run test.ipynb, etl.ipynb, or etl.py until you have run create_tables.py at least once to create the sparkifydb database, which these other files connect to.

## Data Modeling with Postgres

This project is a data modeling project for a music startup - called Sparkify. I was tasked with creating a database in Postgres with tables that I have to model with efficient star schema and ETL pipeline to be able to get the data from the log and data files into the database.

For the star schema, there are 1 fact table and 4 dimesnsion tables. The fact table - Songplays table - captures the records in logdata file associated with song plays. The dimensions tables are the users table - used to store the app users records, songs table - used to store the songs in the music database, artists table - used to store the artists in the music database, time table - used to store the broken down timestamps of the records in songplays.

#### How to run the Python Scripts

The project files contain some datafiles in the data folder and six files: test.ipynb, create_tables.py, etl.ipynb, etl.py, sql_queries.py and a README.md file.

The test.ipynb displays the first few rows of each table to let you check the database.
The create_tables.py drops and creates the tables. This file is run to reset the tables before each time you run your ETL scripts.
The etl.ipynb reads and processes a single file from song_data and log_data and loads the data into the tables. It contains detailed instructions on the ETL process for each of the tables.
The etl.py reads and processes files from song_data and log_data and loads them into your tables. 
The sql_queries.py contains all the sql queries, and is imported into the create_tables.py, etl.ipynb and etl.py files.
The README.md provides discussion on this project and it is the current file you are reading from.


Run create_tables.py to create the database and tables.
Run test.ipynb to confirm the creation of the tables with the correct columns. 
Make sure to click "Restart kernel" to close the connection to the database after running the test.ipynb. 
Run the etl.py to reset the tables. 
Run test.ipynb to confirm the records were successfully inserted into each table.

