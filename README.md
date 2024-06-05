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
AviationStack texts.

## Data Model
AviationStack data model.

## Launch Project
https://app.powerbi.com/reportEmbed?reportId=6db999f7-44e4-4c11-a815-7d9da75041cd&autoAuth=true&ctid=461455b5-e6f3-430b-ab4c-9bc4818a4cd3





