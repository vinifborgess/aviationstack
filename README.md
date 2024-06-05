## Aviation Data Engineering Project | Modern Data Engineering E2E Project
Using AviationStack API to obtain historical flight data and perform basic flight data processing and analysis.

## Problem Statement:
Obtain historical flight data and perform basic flight data processing and analysis.

## Architecture:
This architecture is designed/developed to be a robust and detailed product, standardized, and able to re-usability.

```
                +----------------------------------+
                |          Data Extraction         |
                |----------------------------------|
                | AviationStack API                |
                | Params: access_key, airline_iata |
                +----------------+-----------------+
                                 |
                                 v
                +----------------+-----------------+
                |       Data Transformation        |
                |----------------------------------|
                | Parse JSON, Normalize Fields     |
                |                                 |
                +--------+-----------------+-------+
                         |                 |
                         v                 v
                +--------+--------+ +------+------+
                |   CSV Storage   | | SQLite DB   |
                |-----------------| |-------------|
                | Write to CSV    | | Insert Data |
                +--------+--------+ +------+------+
                         |                 |
                         v                 v
                +--------+-----------------+-------+
                |        Data Retrieval            |
                |----------------------------------|
                | Query SQLite DB, Print Results   |
                +----------------------------------+
```
## Tech stack:
Language: Python;
Softwares: AviationStackAPI, Figma, PowerBI.

## More about the data
The following project uses the AviationStack API to access aviation data. Each aviationstack account is assigned a unique access key, known as the master key, which must be used to authenticate requests to the API. You can find your master key in your account dashboard. Each account is assigned only one master key.

If you want to view customized data, enter your key, modify the code, and download the project to your local machine.

To connect to the API, simply attach the access_key parameter to any valid API endpoint URL and set it to your master key. See the example below:

```
https://api.aviationstack.com/v1/flights?access_key=YOUR_ACCESS_KEY
```

Replace YOUR_ACCESS_KEY with your actual master key.

## Data Model
AviationStack data model.

## Launch Project
https://app.powerbi.com/reportEmbed?reportId=6db999f7-44e4-4c11-a815-7d9da75041cd&autoAuth=true&ctid=461455b5-e6f3-430b-ab4c-9bc4818a4cd3





