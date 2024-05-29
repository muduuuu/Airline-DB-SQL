# Airline-Database 
The database consists of multiple tables which needs querying to be done in order to extract relavant information.

# Table of Contents
Introduction </br>
Database Schema</br>
Queries</br>
Prequisites</br>
Author</br>

# Database schema
CREATE TABLE aircrafts_data ( </br>
    aircraft_code character(3) NOT NULL,</br>
    model jsonb NOT NULL,</br>
    range integer NOT NULL,</br>
    CONSTRAINT aircrafts_range_check CHECK ((range > 0))</br>
);</br>
CREATE TABLE airports_data (</br>
    airport_code character(3) NOT NULL,</br>
    airport_name jsonb NOT NULL,</br>
    city jsonb NOT NULL,</br>
    coordinates point NOT NULL,</br>
    timezone text NOT NULL</br>
);</br>
CREATE TABLE boarding_passes (</br>
    ticket_no character(13) NOT NULL,</br>
    flight_id integer NOT NULL,</br>
    boarding_no integer NOT NULL,</br>
    seat_no character varying(4) NOT NULL</br>
);</br>
Other schemas can be obtained via the provided sql file
# Queries
This section contains a list of SQL queries performed on the database to extract meaningful information. Examples include: </br>

Finding all flights between two cities.</br>
Counting the number of flights per airline.</br>
Listing all passengers on a specific flight.</br>
Calculating the average delay time for each airline.</br>
Identify details of the longest flight (using flights table) </br>
30 Other queries were performed.
## Prerequisites
SQL database management system (e.g., MySQL, PostgreSQL, SQLite)
# Author
Dataset: https://www.kaggle.com/datasets/fiazbhk/airline-data-analysis
# Details
Name: Mudassir Hayath </br>
Email: mudassirhayath30@gmail.com </br>
Let's connect on LinkedIn: https://linkedin.com/in/mudassir-hayath/
