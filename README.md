#Dependencies
requests
pandas
pyodbc
SQLAlchemy
#Configuration
The script uses Windows Authentication to connect to the SQL Server database. Ensure that the ODBC Driver 17 for SQL Server is installed.
##Script Breakdown
#HTTP Request:

The script makes an HTTP GET request to the Premier League website to retrieve football player statistics.
#Check Data and Display:

If the request is successful, the script extracts player information and prints it.
#Database Connection and Data Import:

If the request is successful, the script establishes a connection to a local SQL Server database using Windows Authentication and inserts player data into the database.
#Database Commit and Closure:

The script commits the changes to the database, closes the cursor, and closes the database connection.
Database Structure
The script assumes the existence of a local SQL Server database named PremierLeagueStats and a table named FootballStats with columns: Index, PlayerName, TeamName, and Goals.
