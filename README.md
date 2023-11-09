## Project Summary:

A data project to showcase the ability to take a significant amount raw data through all activities within a data pipeline, serve the data to a persistent data store, and then glean insight from the data via a fully interactive web-based visualization mechanism.

### <u>Data Pipeline</u>

#### Generation:

NOAA data repository of .csv files by weather station and year. The actual files contain the lowest level of weather observation data with many attributes that are free of use to access.  Python scripts selectively pulling in data to store locally for all required locations and periods. Using the threading and urlib.request libraries for maximum efficiency and speed.

#### Storage:

Maintain the stripped down .csv on a local machine, and consolidate to parquet files for ingestion into the pipeline and also to serve as a backup in case of failure (reproduction.). Also, in case the utilization of files and process for production to a different database engine (MySQL).

#### Ingestion:

With the parquet files, by year, the next step of the process is to utilize these files to feed the transformation process.

#### Transformation:

All of the transformation activities are done through python generator functions, list and dictionaries before being committed to the Postgres database tables.  The sqlalchemy orm is relied upon for ulitmate processing.

#### Serving:

The final product within the data pipeline stage is to have a persistent data store currently via the Postgres database engine either on a local machine and/or on the www.render.com cloud platform the serve the next step(s).

#### Data Analysis: Exploratory

Harnessing a fully finished Postgres database, directly, via the Bokeh visualization library to explore the data in an interactive web-browser.

##### Python Libararies Utilized:

<u>Standard</u> - configparser, os, time, threading, urllib.request, datetime, csv, sys, logging

<u>Third Party</u> - polars, pyspark, sqlalchemy, psycopg2, pandas, requests

##### Other Resources Utilized:

- Mac Command Line

- Postgres

- SQL

- PyCharm

- Visual Studio Code

- JupyterLab

- Render

- Heroku

- Git & GitHub

- Pip

- Home Brew

- HTML5up.net

  

