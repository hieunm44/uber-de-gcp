# Uber Data Pipeline with GCP

## Overview
This repo is a tutorial of how to build an ETL pipeline on GCP. The used data is Uber's trip records.

## Tech Stack
- **Infrastructure**: Google Compute Engine
- **Pipeline**: Mage AI
- **Data Processing**: pandas
- **Data Lake**: Google Cloud Storage
- **Data Warehouse**: Google BigQuery
- **BI Tool**: Looker Studio

## Data Flow
1. **Extract**: The data file is at `data/uber_data.csv`. The original data is provided here: https://www.nyc.gov/site/tlc/about/tlc-trip-record-data.page
2. **Transform**: Transform raw data using `mage` which will be installed on a Compute Engine Instance
3. **Load**: Load transformed data into tables in a Dataset in BigQuery
4. **Analytic**: Analyze data using Looker Studio


## Usage
1. Check file `UberDataPipeline.ipynb` to have an overview of how data will be processed
2. Follow the steps in file `Tutorial.ipynb`