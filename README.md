# NELA-GT-2019

This repository contain examples of how to use the NELA-GT-2019 data set with Python 3.

__For more details about this data set, check the paper__:
`<link>`

If you use this dataset in your work, please cite us as follows:
`<citation>`

## Data

|Metadata||
---|---
Dataset name | `NELA-GT-2019`
Formats|`JSON`, `Sqlite3`
No. of articles | `1.12M`
No. of sources | `260`
Collection period| `2019-01-01` to `2019-12-31`

### Fields

Each data point collected corresponds to an article and contains the fields described below.

|Field | Type | Description|
---|---|---
`id` | string | ID of the article
`date` | string | date of publication (`YYYY-MM-DD`)
`source` | string | name of the source
`title` | string | article headline
`author` | string | author who signed the article
`published` | string | date time string as provided by source
`published_utc` | integer | unix timestamp of publication
`collection_utc` | integer | unix timestamp of collection date

### Aggregated labels

We provide aggregated labels based on Media Bias/Fact Check reports, classifying each source as:

* _Reliable_ - class 0
* _Mixed_ - class 1
* _Unreliable_ - class 2

These labels can be found in `labels.csv`


## Examples
###  load-sqlite3.py

* How to load the data from the Sqlite3 database using SQL queries.
  + Loading data from single or multiple sources from the database
  + Loading data from the database into a Pandas dataframe

Usage:
```
python3 load-sqlite3.py <path-to-database>
```

###  load-json.py

* How to load NELA in JSON format with Python 3.
  + Loading a single source's JSON
  + Loading a directory of NELA JSON files - **WARNING**: this may take lots of memory

Usage:
```
python3 load-json.py <path-to-file>
```
