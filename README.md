# NELA-GT_2019

This repository contain examples of how to use the NELA-GT-2019 data set with Python 3.

## load-sqlite3.py

* How to load the data from the Sqlite3 database using SQL queries.
  + Loading data from single or multiple sources from the database
  + Loading data from the database into a Pandas dataframe

Usage:
```
python3 load-sqlite3.py <path-to-database>
```

## load-json.py

* How to load NELA in JSON format with Python 3.
  + Loading a single source's JSON
  + Loading a directory of NELA JSON files - **WARNING**: this may take lots of memory

Usage:
```
python3 load-json.py <path-to-file>
```
