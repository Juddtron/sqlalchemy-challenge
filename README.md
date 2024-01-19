sqlalchemy-challenge

This project uses Python and SQLAlchemy to do basic data exploration and analysis of an SQLite climate database. All analysis is done using SQLAlchemy (ORM queries), Pandas, and Matplotlib. It also provides an API (designed using Flask) for querying this climate data.



Part I: Exploratory Climate Analysis

This part of the project analyzes Hawaii precipitation and weather station data, and produces visualizations of rainfall and temperature patterns. It also supports the planning of visits to Hawaii with:

local precipitation summaries for each of the local weather stations and
temperature dailies for a flexible range of trip dates.
It consists of:

a SQLite database (Resources/Hawaii.sqlite)
a Jupyter notebook (sqlalchemy-challenge/climate_analysis.ipnyb) that uses SQLAlchemy, Python Pandas and MatPlotlib to analyze and visualize this data.
Bar charts, a histogram and an area chart that are visible within the notebook and also stored as .png files in the sqlalchemy-challenge folder.



Part II: Climate App

This part of the project surfaces several SQLAlchemy precipitation and temperature queries in an API using a Python Flask app:

/
Home page
/api/v1.0/precipitation
Daily precipitation totals for last year
/api/v1.0/stations
Active weather stations
/api/v1.0/tobs
Daily temperature observations for the WAIHEE weather station
/api/v1.0/trip/yyyy-mm-dd
Min, average & max temperatures for the range beginning with the provided start date through 08/23/17
/api/v1.0/trip/yyyy-mm-dd/yyyy-mm-dd
Min, average & max temperatures for the range beginning with the provided start - end date range
